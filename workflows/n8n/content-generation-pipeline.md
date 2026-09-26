# Content Generation Pipeline

## Nodes

### 1. Manual Trigger
Starts a test run.

### 2. Input
Provide topic, source text, target languages and platforms.

### 3. AI Generation
Ask the model to return strict JSON containing:

- hook
- title
- script
- caption
- CTA
- hashtags
- visual direction

### 4. Validation
Reject the result when required fields are missing or malformed.

### 5. Translation
Generate platform-ready translations for each requested language.

### 6. Human Approval
Present the generated package for review.

### 7. Publishing Adapter
Only approved content reaches the publishing layer.

### 8. Analytics
Store publication identifiers and later performance metrics.

## Important

The workflow intentionally separates generation from publishing. This makes testing safer and allows multiple platforms to reuse the same approved content package.
