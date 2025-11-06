# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted (by Technical Writer with input from PM and developers)
- Rollback / mitigation plan documented (reviewed by SRE)
- Smoke tests prepared
- User documentation updated (Technical Writer)

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable) — SRE responsibility
- [ ] Deploy to staging and run smoke tests — SRE monitors
- [ ] Deploy to production (automated pipeline preferred) — SRE oversight
- [ ] Run post-deploy verifications — SRE validates system health
- [ ] Announce release to stakeholders and support — PM and Technical Writer collaborate

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify SRE on-call
  - SRE leads rollback to last known-good release if necessary
  - Triage root cause and capture action items
  - Technical Writer updates release notes with known issues if needed

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:

**Prepared by**: Technical Writer in collaboration with PM and development team.
**Reviewed by**: Product Manager, Tech Lead, and SRE for accuracy and completeness.
