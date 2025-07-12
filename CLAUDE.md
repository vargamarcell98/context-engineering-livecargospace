# Claude.md

### 🔄 Project Awareness & Context

- **Always read `PLANNING.md`** at the start of a new conversation to understand the project's architecture, goals, style, and constraints.
- **Check `TASK.md`** before starting a new task. If the task isn’t listed, add it with a brief description and today’s date.
- **Follow consistent naming conventions, file structure, and component architecture** as outlined in `PLANNING.md`.
- **Use the existing `Next.js` app structure**, including pages, components, hooks, and utilities.

---

### 🧱 Code Structure & Modularity

- **Never create a file longer than 300 lines of code.** Break into smaller modules or components.
- **Group related logic** using folders such as:
  - `components/` – Reusable UI elements (e.g. GanttChart.tsx, LoadCard.tsx)
  - `lib/` – Utility functions and API helpers
  - `hooks/` – Custom React hooks
  - `pages/` – Route-specific pages
  - `types/` – TypeScript interfaces and types

- **Use clear, consistent imports**, and prefer absolute imports (`@/lib`, `@/components`) over relative imports.

- **Environment variables** should be stored in `.env.local` and accessed via `process.env`.

---

### 🧪 Testing & Reliability

- **Write unit and integration tests** using **Vitest** (or **Jest**) for logic-heavy functions, custom hooks, and API routes.
- **Use Playwright or Cypress** for end-to-end testing of user flows (e.g. drag-and-drop, modal forms, login).
- Store tests under the `__tests__/` or `tests/` directory mirroring the source structure.
- Each test should include:
  - 1 success case
  - 1 edge case
  - 1 failure case (if meaningful)

---

### ✅ Task Completion

- **Mark completed tasks in `TASK.md`** after finishing them.
- Add any discovered subtasks or bugs to `TASK.md` under a "Discovered During Work" section.

---

### 📎 Style & Conventions

- **Use TypeScript** as the primary language.
- **Follow ESLint and Prettier rules**, auto-format on save.
- **Use Tailwind CSS** for styling.
- For backend:
  - **Use Supabase** for database, authentication, and API layer
  - **Use `zod`** for input validation

- Write **JSDoc or inline comments** for complex logic.

---

### 📚 Documentation & Explainability

- **Update `README.md`** whenever features are added or configuration/setup changes.
- **Comment all non-obvious code** to ensure it is understandable for a mid-level developer.
- **Use `// Reason:` inline comments** for complex or non-intuitive logic.

---

### 🧠 AI Behavior Rules

- **Never assume missing context. Ask questions when uncertain.**
- **Never hallucinate libraries, paths, or functions** – only use known, verified packages.
- **Confirm file paths, components, and APIs exist** before referencing them in new code.
- **Do not overwrite or delete existing logic** unless explicitly instructed or listed in `TASK.md`.
