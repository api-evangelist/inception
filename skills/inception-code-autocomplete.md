---
name: Inline code autocomplete and next-edit with Mercury Edit 2
description: Use the FIM and edit completion endpoints to generate IDE-style inline code completions and predicted next edits with Mercury Edit 2.
api: openapi/inception-openapi-original.json
operations: [createFimCompletion, createEditCompletion]
method: generated
generated: '2026-07-19'
---

# Inline code autocomplete and next-edit with Mercury Edit 2

Two code endpoints, both on model `mercury-edit-2` (32K context).

## Fill-in-the-middle (autocomplete)
1. `createFimCompletion` — `POST /v1/fim/completions` with `{ "model": "mercury-edit-2", "prompt": "<prefix>", "suffix": "<text after cursor>", "max_tokens": 1000 }`.
2. Read the inserted code from `choices[0].text`. Set `"stream": true` for `FimCompletionChunk` deltas.
3. Tool calling and function calling are NOT supported on FIM.

## Next-edit prediction
1. `createEditCompletion` — `POST /v1/edit/completions` with a single user message whose content includes the required edit prompt tags: `<|recently_viewed_code_snippets|>`, `<|current_file_content|>`, `<|code_to_edit|>`, `<|cursor|>`, and `<|edit_diff_history|>`.
2. Read the predicted edit from `choices[0].message.content`.

## Rules
- Both endpoints are text-only and latency-optimized; prefer them over chat for editor flows.
- Same OpenAI error envelope and 429/503 backoff rules as chat (see `errors/` and `conventions/`).
- Editor integrations: Cursor, Zed, Kilo Code, Roo Code, OpenCode (see docs/resources).
