---
layout: default
title: Medicine × Cloud Security (Hospital Occupancy API)
---

# 🏥 Medicine × Cloud Security (Hospital Occupancy API)

HIPAA-aware API providing hospital bed availability to authorized staff with MFA and compliance drift monitoring.

## Quick Links
- [Solutions Architecture Document (SAD)](SAD.md)
- [Architecture Decision Record (ADR)](ADR.md)

## Stack
API Gateway · Lambda · DynamoDB (KMS) · Cognito (MFA) · AWS Config · CloudWatch · tfsec

## Security Layers
- **Preventive:** Cognito MFA, IAM least privilege, KMS
- **Detective:** CloudWatch logs & metrics, AWS Config rules
- **Responsive:** Lambda auto-remediation for drifted S3, CI workflow gating
