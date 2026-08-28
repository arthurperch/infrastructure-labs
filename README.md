# Infrastructure Production Labs

**Arthur Perchatkin** · Cloud Systems Administrator / Infrastructure portfolio

**Live index:** https://arthurperch.github.io/infrastructure-labs/

Professional lab index for **infrastructure, DevOps, and SRE** screeners — built to show production-grade cloud + GPU automation.

Each item links to a dedicated GitHub repo with setup detail, runbooks, and proof.

---

## Lab list

| # | Lab | What it shows | Repo |
|---|---|---|---|
| 01 | **GPU Validation Pipeline** | One pipeline, two repos: NVML health checks, CUDA burn, and network validation on the node side, feeding a serverless gate (Lambda + API Gateway + DynamoDB) that decides PROVISION / HOLD / RMA | [node side](https://github.com/arthurperch/gpu-validation) + [control plane](https://github.com/arthurperch/gpu-onboarding-gate) |
| 02 | **AWS Security Auditor** | boto3 IAM / EC2 / S3 / SG compliance checks | [aws-security-auditor](https://github.com/arthurperch/aws-security-auditor) |
| 03 | **Gridwatch** | Network security monitoring — connection snapshots + detection rules + alert sinks | [gridwatch](https://github.com/arthurperch/gridwatch) |
| 04 | **flask-mcp-server** | AI ↔ Flask ↔ AWS automation via MCP | [flask-mcp-server](https://github.com/arthurperch/flask-mcp-server) |

---

## How a hiring manager should use this

1. Skim the numbered list — *hardware validation → control plane → IaC → security → monitoring → automation*.
2. Click any repo.
3. Look for **runbooks**, **verify scripts**, and a clear **done** definition.
4. Ask interview questions from the tags (NVML, PCIe, Terraform, Lambda, IAM, boto3, Ansible, psutil).

---

## Suggested resume block

```
Documented Labs
GPU Validation Fleet — NVML, CUDA burn, network checks, Ansible
GPU Onboarding Gate — Lambda + API Gateway + DynamoDB (PROVISION / HOLD / RMA)
Cloud Infrastructure — Terraform + LocalStack (S3, DynamoDB, Lambda, IAM)
AWS Security Auditor — boto3 IAM / EC2 / S3 / SG checks
Gridwatch — network security monitoring (psutil + detection rules)
```

---

## Stack themes

- **Hardware validation:** NVML, CUDA, PCIe link state, burn testing
- **Orchestration:** Ansible, Terraform (IaC)
- **Cloud:** AWS (Lambda, API Gateway, DynamoDB, IAM, S3), LocalStack
- **Security / Monitoring:** IAM, network security monitoring (Gridwatch)
- **Automation:** Python, boto3
- **AI / Platform:** MCP (flask-mcp-server)

---

## Author

**Arthur Perchatkin**

GitHub: [arthurperch](https://github.com/arthurperch)

Certifications: AWS Solutions Architect Associate · AWS CloudOps Engineer Associate

Lab environments only. No production secrets.
