---
layout: default
title: Consumer Health/Wellness × Cloud Security
---

# 🧴 Consumer Health/Wellness × Cloud Security

A secure ingredient lookup API that enforces least-privilege IAM, encryption at rest, and runtime compliance.

## Quick Links
- [Solutions Architecture Document (SAD)](SAD.md)
- [Architecture Decision Record (ADR)](ADR.md)

## Stack
API Gateway · Lambda · DynamoDB (KMS) · AWS Config · WAF · tfsec

## Security Layers
- **Preventive:** tfsec scanning, IAM least privilege, KMS, WAF (OWASP + rate limit)
- **Detective:** AWS Config (CIS) compliance monitoring
- **Responsive:** WAF runtime blocking, CI workflow gating
