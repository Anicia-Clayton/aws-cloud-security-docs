---
layout: default
title: AWS Cloud Security Portfolio
---

# AWS Cloud Security Portfolio

This portfolio showcases **secure-by-design AWS architectures** across three domains:
- 🧴 **Consumer Health/Wellness** — Secure ingredient lookup API
- 🏫 **Education (Homeschool Platform)** — Identity & privacy for global learners
- 🏥 **Medicine (Hospital Occupancy API)** — HIPAA-aware access with continuous compliance

## 🔐 Security Layers

### 🛡️ Preventive
- **tfsec** IaC scanning (pre-deployment)
- **IAM least privilege** for all roles/policies
- **KMS encryption** for DynamoDB
- **WAF** managed rules + **rate limiting** (public APIs)

### 🔍 Detective
- **AWS Config** conformance pack (CIS AWS Foundations)
- **CloudTrail** for change and access auditing
- **CloudWatch Logs & Metrics** for runtime visibility

### 🔁 Responsive
- **Lambda auto-remediation** for common drift (e.g., S3 encryption/public access)
- **Cognito MFA** and **JWT authorizers**
- **GitHub Actions workflow gating** (block merges on critical tfsec findings)

## 📂 Projects
- [🧴 Consumer Health/Wellness × Cloud Security](projects/consumer-secure-ingredient-api/_index.md)
- [🏫 Education × Cloud Security (Homeschool Platform)](projects/education-secure-homeschool-api/_index.md)
- [🏥 Medicine × Cloud Security (Hospital Occupancy API)](projects/medicine-secure-hospital-api/_index.md)
