---
layout: default
title: Education × Cloud Security (Homeschool)
---

# 🏫 Education × Cloud Security (Homeschool Platform)

Secure, private API for high-travel homeschool families: role-based access and encrypted learner data.

## Quick Links
- [Solutions Architecture Document (SAD)](SAD.md)
- [Architecture Decision Record (ADR)](ADR.md)

## Stack
API Gateway · Lambda · DynamoDB (KMS) · Cognito (roles) · AWS Config · tfsec

## Security Layers
- **Preventive:** Cognito group-based access, least-privilege IAM, KMS
- **Detective:** AWS Config CIS pack (no public resources, encryption)
- **Responsive:** JWT authorizers, CI workflow gating
