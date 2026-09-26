# Generic n8n Content Pipeline

## Workflow

1. Manual Trigger / Webhook
2. Input Content
3. AI Generation
4. Structured Output Validation
5. Translation
6. Human Approval
7. Publishing
8. Analytics Capture

## Suggested input

```json
{
  "topic": "Example topic",
  "source_text": "Original source content",
  "target_languages": ["fr", "en", "es"],
  "platforms": ["tiktok", "instagram", "youtube"]
}
```

## Suggested generated output

```json
{
  "hook": "...",
  "script": "...",
  "caption": "...",
  "cta": "...",
  "hashtags": ["..."],
  "translations": {
    "fr": {},
    "en": {},
    "es": {}
  }
}
```

The publishing adapter should be isolated from generation so the same content can be reused across multiple platforms.
