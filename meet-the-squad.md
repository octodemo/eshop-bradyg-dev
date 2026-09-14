# Meet the Squad

**Naming mode:** Descriptive

This is the automatically Cast Squad for **octodemo/eshop-bradyg-dev**, a reference .NET
microservices e-commerce application built on .NET Aspire.

## The Team

| Name | Role | Specialty | How to talk |
| --- | --- | --- | --- |
| Lead | Team Lead | Cross-service architecture, Aspire composition | `@copilot` mention or `squad` label, then describe architectural or cross-cutting concerns |
| Backend | Backend Engineer | ASP.NET Core APIs, EF Core, event integration | Describe the service (Ordering, Catalog, Basket, etc.) and the API/domain change needed |
| Frontend | Frontend Engineer | Blazor WebApp, MAUI ClientApp, HybridApp | Describe the UI/UX change and target client |
| DevOps | DevOps/Platform Engineer | Aspire AppHost, container builds, CI | Describe the pipeline, build, or orchestration issue |
| Test | Test Engineer | xUnit suites, Playwright e2e | Describe the missing coverage or failing test |
| Security | Security Engineer | Identity/auth, credentials, dependency risk | Describe the auth flow or dependency concern |

## How to Work With Your Squad

- Apply the `squad` label (color `9B8FCC`) to an issue or PR to bring it into the Squad's queue.
- Use `/squad triage`, `/squad plan`, and `/squad activate` to move proposals through the lifecycle.
- See `.squad/routing.md` for the exact work-type-to-specialist routing table.

## What Happened Here

This Squad was automatically Cast from repository analysis:

- **Languages/frameworks:** C#/.NET (Aspire, ASP.NET Core, EF Core, MAUI, Blazor), TypeScript
  (Playwright end-to-end tests)
- **Structure:** A multi-service solution under `src/` (Ordering, Catalog, Basket, Identity,
  Payment, Webhooks, and clients) orchestrated by `src/eShop.AppHost`
- **CI/CD:** GitHub Actions workflows for PR validation and Playwright end-to-end testing
- **Rationale:** Six roles were selected — one Lead for cross-service architecture, Backend and
  Frontend for the two dominant implementation surfaces, DevOps for Aspire/container/CI concerns,
  Test for the sizeable `tests/` and `e2e/` suites, and Security for the dedicated Identity service
  and credential-scanning configuration.

---

*Cast on 2026-09-14.*
