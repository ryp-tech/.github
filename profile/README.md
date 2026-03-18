# Rest Your Paws — Engineering

Internal repos for the RYP tech platform. Sugar CRM integrations, Cloud Run microservices, data pipelines, and web forms.

## Getting Started

**New to the team?** Start here:

1. **[`ryp-dev-docs/onboarding.md`](https://github.com/ryp-tech/ryp-dev-docs/blob/main/onboarding.md)** — Full setup guide: GCP access, Sugar credentials, local dev, deploying to Cloud Run, creating new projects
2. **[`ryp-dev-docs/CLAUDE.md`](https://github.com/ryp-tech/ryp-dev-docs/blob/main/CLAUDE.md)** — Org-wide rules, project map, secrets, deployment patterns
3. **[`ryp-dev-docs/sugar-crm-guide.md`](https://github.com/ryp-tech/ryp-dev-docs/blob/main/sugar-crm-guide.md)** — Sugar CRM REST API reference (auth, modules, field mappings, filter syntax)

## Using Claude Code

We use [Claude Code](https://docs.anthropic.com/en/docs/claude-code) as our AI coding assistant. Every repo has a `CLAUDE.md` file that gives Claude context about the project. The shared knowledge lives in [`ryp-dev-docs`](https://github.com/ryp-tech/ryp-dev-docs) — clone it alongside your project repos so Claude Code can reference it:

```
~/ryp-projects/
├── ryp-dev-docs/        ← clone this first
├── client-portal/
├── VFF/
└── your-project/
```

## Key Repos

| Repo | What It Is |
|------|-----------|
| [`ryp-dev-docs`](https://github.com/ryp-tech/ryp-dev-docs) | Shared docs, Sugar API guide, onboarding |
| [`client-portal`](https://github.com/ryp-tech/client-portal) | Aftercare consent & payment form |
| [`clinic-portal`](https://github.com/ryp-tech/clinic-portal) | Vet clinic relationship portal |
| [`VFF`](https://github.com/ryp-tech/VFF) | Vet Feedback Form |
| [`med_records`](https://github.com/ryp-tech/med_records) | Medical Records form |
| [`ryp-pipelines`](https://github.com/ryp-tech/ryp-pipelines) | ETL: Sugar → BigQuery → Xero |
| [`RSS`](https://github.com/ryp-tech/RSS) | Vet calendar sync |
| [`vet-email-agent`](https://github.com/ryp-tech/vet-email-agent) | AI email agent for vet referrals |
| [`ryp-supply-form`](https://github.com/ryp-tech/ryp-supply-form) | Internal supply ordering |
| [`ryp-invoicing`](https://github.com/ryp-tech/ryp-invoicing) | PDF receipt generator |

## Stack

**Backend:** Python 3.11, FastAPI, Uvicorn | **Frontend:** React 18, TypeScript, Vite, Tailwind | **CRM:** Sugar CRM (REST API) | **Cloud:** Google Cloud Run, BigQuery, Secret Manager | **CI/CD:** Manual deploys via `gcloud` CLI
