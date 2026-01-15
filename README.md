# Nexus Repository Manager 3 – Single-Instance Helm Chart

## Important Notice

This repository is **NOT an official Sonatype project**.

It is a **personally maintained copy** of Sonatype’s **archived single-instance Helm chart**.  
The original official repository is no longer maintained.

This chart is provided **as-is** and **must not be considered production-ready**.

---

## Disclaimer and Risk Warning

- No official Sonatype support
- No guarantees of stability or data safety
- Not continuously tested
- Embedded database may become corrupted in container environments

**Use entirely at your own risk.**

---

## Critical Warning from Sonatype

Sonatype strongly warns that running Nexus Repository in containers with the embedded database can lead to database corruption.

For Kubernetes deployments, **using an external PostgreSQL database is strongly recommended**.

Single-instance deployments are inherently unsafe.

---

## Strongly Recommended Alternative (Official)

For any production or long-term usage, **use Sonatype’s officially maintained High Availability (HA) Helm chart**:

https://github.com/sonatype/nxrm3-ha-repository/tree/main/nxrm-ha

The HA chart is the **only supported and production-grade option**.

---

## Intended Use Only

This chart is suitable for:
- Development
- Testing
- Learning
- Temporary or disposable environments

**Not suitable for production.**

---

## Example Installation

```bash
helm repo add nexus-repository-manager https://moechs.github.io/nexus-repository-manager/
helm install nexus-repository-manager nexus-repository-manager/nexus-repository-manager
```
