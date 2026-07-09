# Zero-Trust Identity Governance Platform on Microsoft Entra ID

An end-to-end identity governance architecture built on Microsoft Entra ID, aligned to the SC-300 (Microsoft Identity and Access Administrator) 

Core design principle: **credentials should be short-lived, and privilege should be earned on demand — never standing.**

**Full write-up and More project:** https://hanqin-lyu.github.io/

---

## What's in this repo

This repo holds the raw evidence behind the project — screenshots showing each step actually configured and tested, not just described. Organized to match the four build phases:

```
01-workload-identity-federation/
    Workload Identity Federation (GitHub Actions OIDC) vs. Managed Identity
    — zero-secret authentication, tested both ways against the same Key Vault

02-conditional-access/
    Six layered Conditional Access policies — baseline MFA, phishing-resistant
    MFA for privileged roles, risk-based response, legacy auth blocking

03-privileged-identity-management/
    PIM Eligible role conversions — both Entra directory roles
    (Global Administrator, Privileged Role Administrator) and Azure
    resource roles (Key Vault, Automation Account)

04-entitlement-management-and-lifecycle-workflows/
    Access Package request/approval/expiry flows, plus full
    Joiner-Mover-Leaver Lifecycle Workflow automation
```

Each folder's screenshots are numbered in the order you'd walk through that phase, so they read top-to-bottom as a story rather than a random screenshot dump.

## How to read this repo

Start with the [project page](https://hanqin-lyu.github.io/Projects/Zero-Trust%20Identity%20Governance%20Platform%20on%20Microsoft%20Entra%20ID.html) for the architecture and the reasoning. Come back here for the underlying proof — every claim on that page traces back to a screenshot in one of these folders.
