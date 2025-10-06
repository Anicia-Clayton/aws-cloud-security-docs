---
layout: default
title: AWS Cloud Security Portfolio
---

<!-- Hero (Cayman keeps its banner; this adds a brief intro) -->
# AWS Cloud Security Portfolio

This portfolio showcases **secure-by-design AWS architectures** across three domains.

<!-- Card Grid (restores the original visual) -->
<div style="display:grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap:16px; padding:24px; max-width:1100px; margin: 0 auto 24px auto;">
  <div style="background:#fff; border-radius:12px; box-shadow:0 6px 20px rgba(0,0,0,.08); padding:18px; border:1px solid #eaeef2;">
    <div style="font-size:12px; margin-bottom:6px;">
      <span style='background:#eaeef2;border-radius:999px;padding:2px 6px;'>Consumer</span>
      <span style='background:#eaeef2;border-radius:999px;padding:2px 6px;'>WAF</span>
      <span style='background:#eaeef2;border-radius:999px;padding:2px 6px;'>tfsec</span>
    </div>
    <h3 style="margin:6px 0;">Consumer Wellness API</h3>
    <p>Serverless API with WAF protection and Config compliance.</p>
    <p><b>Stack:</b> API GW · Lambda · DynamoDB (KMS)</p>
    <p><a href="projects/consumer-secure-ingredient-api/">View project →</a></p>
  </div>
  <div style="background:#fff; border-radius:12px; box-shadow:0 6px 20px rgba(0,0,0,.08); padding:18px; border:1px solid #eaeef2;">
    <div style="font-size:12px; margin-bottom:6px;">
      <span style='background:#eaeef2;border-radius:999px;padding:2px 6px;'>Education</span>
      <span style='background:#eaeef2;border-radius:999px;padding:2px 6px;'>Cognito</span>
      <span style='background:#eaeef2;border-radius:999px;padding:2px 6px;'>JWT</span>
    </div>
    <h3 style="margin:6px 0;">Education Homeschool API</h3>
    <p>Role-based access for parents, students, tutors with Cognito.</p>
    <p><b>Stack:</b> API GW · Lambda · DynamoDB (KMS)</p>
    <p><a href="projects/education-secure-homeschool-api/">View project →</a></p>
  </div>
  <div style="background:#fff; border-radius:12px; box-shadow:0 6px 20px rgba(0,0,0,.08); padding:18px; border:1px solid #eaeef2;">
    <div style="font-size:12px; margin-bottom:6px;">
      <span style='background:#eaeef2;border-radius:999px;padding:2px 6px;'>Medicine</span>
      <span style='background:#eaeef2;border-radius:999px;padding:2px 6px;'>MFA</span>
      <span style='background:#eaeef2;border-radius:999px;padding:2px 6px;'>Config</span>
    </div>
    <h3 style="margin:6px 0;">Hospital Occupancy API</h3>
    <p>HIPAA-aware access with MFA and continuous compliance.</p>
    <p><b>Stack:</b> API GW · Lambda · DynamoDB (KMS)</p>
    <p><a href="projects/medicine-secure-hospital-api/">View project →</a></p>
  </div>
</div>

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
- [🧴 Consumer Health/Wellness × Cloud Security](projects/consumer-secure-ingredient-api/)
- [🏫 Education × Cloud Security (Homeschool Platform)](projects/education-secure-homeschool-api/)
- [🏥 Medicine × Cloud Security (Hospital Occupancy API)](projects/medicine-secure-hospital-api/)
