---
name: Run a tool-calling agent turn with Mercury 2
description: Use Mercury 2 tool calling on the chat endpoint to let the model invoke functions and orchestrate multi-step agent workflows.
api: openapi/inception-openapi-original.json
operations: [createChatCompletion]
method: generated
generated: '2026-07-19'
---

# Run a tool-calling agent turn with Mercury 2

Tool calling is supported on `createChatCompletion` (chat only — not FIM or edit).

## Steps
1. `createChatCompletion` — `POST /v1/chat/completions` with `model: mercury-2`, your `messages`, and a `tools` array of function definitions (`{ "type": "function", "function": { name, description, parameters } }`).
2. If the model wants a tool, the response `choices[0].message.tool_calls[]` lists calls with `function.name` and JSON `function.arguments`.
3. Execute each tool in your own code, then append a `{"role":"tool", "tool_call_id":"...", "content":"<result>"}` message.
4. Call `createChatCompletion` again with the extended message list to get the final answer in `choices[0].message.content`.

## Structured output
To force a typed result instead of free text, set `response_format` to `{ "type": "json_schema", "json_schema": {...} }`. See `conventions/inception-conventions.yml` and https://docs.inceptionlabs.ai/capabilities/tool-use.

## Rules
- Keep a stable `tool_call_id` mapping between the model's request and your tool result message.
- Handle `400 invalid_request_error` for malformed tool schemas; retry `429`/`503` with backoff.
