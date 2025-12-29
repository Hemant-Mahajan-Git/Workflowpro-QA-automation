# Workflowpro-QA-automation
# WorkFlow Pro – QA Automation Challenge

## Overview
This repository contains my solution for the QA Automation Challenge for **WorkFlow Pro**,
a multi-tenant B2B SaaS project management platform.

The solution demonstrates:
- Debugging and fixing flaky UI automation tests
- Designing a scalable automation framework
- API + UI + Mobile integration testing
- Multi-tenant security and data isolation validation

---

## Tech Stack
- Python
- Pytest
- Playwright
- Requests (API Testing)
- BrowserStack (Mobile Testing)

---

## Repository Structure
The framework is organized into UI, API, and Integration tests using Page Object Model
and reusable utilities.

---

## Part 1: Flaky Test Resolution
Issues fixed:
- Missing waits for dynamic elements
- Hard URL assertions
- CI vs local execution timing issues
- Tenant-specific loading delays

Improvements:
- Explicit waits using Playwright `expect`
- Fixture-based browser handling
- Stable navigation validation

---

## Part 2: Framework Design
Key features:
- Multi-tenant environment support
- Role-based testing (Admin, Manager, Employee)
- Web + Mobile testing
- API automation integration
- CI/CD ready architecture

---

## Part 3: API + UI + Mobile Integration Test
End-to-end flow:
1. Create project via API
2. Verify project in Web UI
3. Verify project on Mobile
4. Validate tenant isolation

---

## Assumptions
- Token-based authentication is available
- Separate test tenants exist
- API cleanup endpoints are supported
- BrowserStack credentials are configured securely

---

## How to Run Tests
```bash
pip install -r requirements.txt
pytest
