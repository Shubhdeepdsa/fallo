## 🔷 Milestone 1: Project Setup & Tech Stack (4–6 hrs)

### 🟢 `#1: Setup TurboRepo Monorepo with pnpm`
- `apps/web` for React frontend  
- `apps/api` for FastAPI backend  
- `packages/ui`, `packages/types` (shared components + schemas)
- Setup `.npmrc`, `.gitignore`, VSCode workspace
- ✅ Commit: "Initialize monorepo with TurboRepo"
- 🧠 Learn: TurboRepo, mono-repo patterns
- 🕒 1–2 hrs

---

### 🟢 `#2: Setup Tailwind, shadcn/ui, and basic routing`
- Add `tailwind.config.js`, PostCSS  
- Add shadcn/ui components (Button, Card, Tabs)
- Setup `react-router-dom` with `/list`, `/calendar`, `/stats`
- ✅ Commit: "Setup frontend scaffold with Tailwind and shadcn"
- 🧠 Learn: atomic UI structure, Tailwind utils
- 🕒 1.5 hrs

---

### 🟢 `#3: PocketBase Setup with Task Collection`
- Download PB binary, run locally  
- Create `tasks` collection with fields: `title`, `desc`, `dueDate`, `frequency`, `isDone`, `category`
- ✅ Commit: "Setup PocketBase schema"
- 🧠 Learn: PocketBase basics, schema design
- 🕒 1 hr

---

## 🔷 Milestone 2: Task List + Auth Integration (6–8 hrs)

### 🟢 `#4: Create Task List Page with React Query`
- Fetch tasks from PB
- Render cards with `title`, `isDone`
- Add checkbox toggle to mark done
- ✅ Commit: "Task list working with real data"
- 🧠 Learn: TanStack Query, REST data modeling
- 🕒 2 hrs

---

### 🟢 `#5: Add Login/Signup UI with PocketBase SDK`
- Use `pb.authWithPassword()` for login  
- Store token in `authStore`, persist with cookies or localStorage
- Show/hide pages based on login status
- ✅ Commit: "Auth working using PocketBase SDK"
- 🧠 Learn: auth flows, PB authStore
- 🕒 2–3 hrs

---

### 🟢 `#6: Setup FastAPI with PocketBase Token Validation`
- Add FastAPI route `/stats`  
- Parse `Authorization` header  
- Validate token via `auth-refresh` route  
- Return mock data if token is valid
- ✅ Commit: "FastAPI route with PB token validation"
- 🧠 Learn: backend auth + FastAPI security
- 🕒 2 hrs

---

## 🔷 Milestone 3: Calendar & Stats View (5–6 hrs)

### 🟢 `#7: Render Tasks on Monthly Calendar`
- Use `react-big-calendar`  
- Convert dueDate → start/end format  
- Add color/marker for completed vs pending
- ✅ Commit: "Calendar view with task events"
- 🧠 Learn: calendar data shaping
- 🕒 2 hrs

---

### 🟢 `#8: Show Mini Daily Summary Stats`
- Show # tasks today, completed, overdue
- Style with shadcn Card components
- ✅ Commit: "Daily summary dashboard"
- 🧠 Learn: data filtering, UX
- 🕒 1.5 hrs

---

### 🟢 `#9: Add Completion Over Time Chart`
- Use `Recharts` to show last 14 days  
- Daily completions bar or line chart
- ✅ Commit: "Analytics chart for task completion"
- 🧠 Learn: charting, insights
- 🕒 2 hrs

---

## 🔷 Milestone 4: Testing & DevOps (8–10 hrs)

### 🟢 `#10: Setup Unit + Integration Tests`
- Install Vitest, @testing-library/react  
- Write test: "Task checkbox toggles status"
- ✅ Commit: "Add unit tests for TaskList"
- 🧠 Learn: test-driven mindset
- 🕒 2 hrs

---

### 🟢 `#11: Add Cypress E2E Test for Task Flow`
- Add login → create → complete task  
- Run in `apps/web/cypress`
- ✅ Commit: "E2E tests for task workflow"
- 🧠 Learn: high confidence integration
- 🕒 3 hrs

---

### 🟢 `#12: Setup GitHub Actions CI`
- Run `pnpm lint`, `pnpm test`, `pnpm build`
- Use `turbo` cache config  
- ✅ Commit: ".github/workflows/ci.yml"
- 🧠 Learn: CI pipelines
- 🕒 2 hrs

---

## 🔷 Optional Bonus Milestones

### `#13: Responsive Mobile Layout with Tailwind`
- Add media queries, stacked layout for phones
- 🕒 2 hrs

### `#14: Add Offline Support with vite-plugin-pwa`
- Cache assets, sync tasks once online
- 🕒 3 hrs

### `#15: Add recurring task materializer (FastAPI cron job)`
- Run once/day to materialize new daily/weekly task instances
- 🕒 4 hrs

