# Security

## Never commit secrets

Do not commit:

- API keys
- OAuth tokens
- passwords
- session cookies
- webhook secrets
- private certificates
- personal data
- production credentials

Store credentials in n8n's credential system or an appropriate secret manager.

## Reporting a vulnerability

Please do not publish sensitive vulnerability details in a public issue.

Contact the repository maintainer privately with:

- a description of the issue
- affected component
- reproduction steps
- potential impact
- suggested mitigation, if known

## Production deployments

This repository contains reusable building blocks. Production credentials, private infrastructure and account-specific configuration should remain outside the repository.
