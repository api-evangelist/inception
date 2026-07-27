---
name: Generate a chat completion with Mercury 2
description: Call the Inception API to generate a conversational response from the Mercury 2 diffusion LLM, optionally streaming the output.
api: openapi/inception-openapi-original.json
operations: [createChatCompletion, listChatModels]
method: generated
generated: '2026-07-19'
---

# Generate a chat completion with Mercury 2

Use this to get a text response from Inception's `mercury-2` model over the OpenAI-compatible chat endpoint.

## Auth
Send `Authorization: Bearer <INCEPTION_API_KEY>`. Get a key at https://platform.inceptionlabs.ai/dashboard/api-keys. Base URL is `https://api.inceptionlabs.ai`.

## Steps
1. (Optional) `listChatModels` — `GET /v1/chat/completions/models` to confirm `mercury-2` is available to your account.
2. `createChatCompletion` — `POST /v1/chat/completions` with `{ "model": "mercury-2", "messages": [{"role":"user","content":"..."}], "max_tokens": 10000 }`.
3. Read the reply from `choices[0].message.content`. Read `usage` for prompt/completion token counts (billing).

## Streaming
Set `"stream": true` to receive `ChatCompletionChunk` deltas as server-sent events; concatenate `choices[0].delta.content`. Set `"diffusing": true` to also observe intermediate denoising states. See `conventions/inception-conventions.yml`.

## Rules
- Mercury 2 is text-only (no image/vision input) and has a 128K context window.
- On `429` (rate_limit_error) or `503` (engine overloaded), retry with exponential backoff — completions are safe to retry (see `conventions/`). There is no idempotency key.
- Errors use the OpenAI error envelope `{ "error": { message, type, param, code } }` — see `errors/inception-problem-types.yml`.
