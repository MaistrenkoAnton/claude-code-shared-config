# CLAUDE.md

## Project Goal

Build a lightweight markdown knowledge base system within 3 days.

Prioritize:

* simplicity,
* readability,
* delivery speed,
* maintainability.

Avoid overengineering.

---

# Core Rules

## 1. Simplicity First

Implement the minimum solution that works.

Do not add:

* plugin systems,
* generic factories,
* repository abstractions,
* event systems,
* unnecessary configuration,
* speculative extensibility.

If a solution feels "enterprise", simplify it.

---

## 2. Filesystem is the Source of Truth

Documents are stored as markdown files.

Do not introduce:

* database patterns,
* ORM abstractions,
* persistence layers designed for SQL databases.

---

## 3. JSON Config Drives the System

The configuration file defines:

* document types,
* fields,
* validation rules,
* UI form structure.

Frontend and backend must follow the config.

---

## 4. Surgical Changes Only

Modify only code directly related to the task.

Do not:

* refactor unrelated code,
* rename unrelated variables,
* reformat unrelated files,
* reorganize project structure without request.

---

## 5. Avoid Premature Abstractions

Do not create abstractions for:

* single implementations,
* single storage providers,
* single use-cases.

Prefer explicit code over generic architecture.

---

## 6. Ask When Unclear

Do not silently assume requirements.

If multiple interpretations exist:

* explain tradeoffs,
* ask clarifying questions.

---

## 7. MVP First

The goal is a working production-capable MVP.

Not a future-proof platform.

Optimize for:

* clarity,
* speed,
* maintainability.

Not theoretical scalability.

---

## 8. Testing Expectations

Prefer:

* focused unit tests,
* clear validation tests,
* minimal integration tests.

Do not generate excessive test scaffolding.

---

## 9. Frontend Guidelines

Use:

* React 18 + Vite 5 + TypeScript,
* shadcn/ui + Tailwind CSS,
* React Hook Form + Zod,
* TanStack Query v5,
* React Router v6.

Keep UI simple and extendable.

Avoid custom design systems.

---

## 10. Backend Guidelines

Use:

* FastAPI,
* Pydantic,
* filesystem-based repositories.

Keep API contracts explicit and simple.
