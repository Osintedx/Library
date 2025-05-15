# Library

A web application developed to manage a library system, track products, and organize operations.

> **Important:** Please read all `ReadMe.md` files in this project completely before starting!

---

## Project Workflow

### Roles

#### Engineers

* Responsible for planning in **Week 1**.
* Must submit **designs and project documentation** by the end of the first week.
* Deliverables include: UI/UX designs, UML diagrams, functional/non-functional requirements, personas, and presentation organization.

#### Developers

* Begin implementation in **Week 2** based on Engineers' submissions.
* Work on frontend and backend components.
* Tasks will be managed via **Jira** — ensure all work is tracked and updated accordingly.

---

## Collaboration Guidelines

* Cross-team collaboration is encouraged. Everyone should understand how the software works — both functionally and in terms of user experience — regardless of their role.
* The application must be runnable on each team member's machine.
* Use Jira for task management, sprint planning, and communication.

---

## Git Workflow (Developers)

* **Do NOT push directly to `master`.**
* Create your own feature branch named after yourself (e.g., `dev-branch-name`).
* Once your work is complete, submit a **pull request to `dev`**.
* Once approved, a pull request can then be made from `dev` to `master`.

---

## Code & Folder Structure

### Naming Conventions

* **Files/Variables:** `camelCase` (except environment config variables)
* **Folders:** `CamelCase` (unless they are abbreviations, e.g., API)

### Project Structure

```
/Database
  ├── /Liquibase
  ├── /Mapper
      ├── /Entities        # TypeORM entities with optional caching logic
      └── /Enums           # e.g., TechCodes.ts

/Webpage
  ├── /Style              # All CSS files
  ├── /Images             # All assets
  ├── /Scripts            # Feature-specific TS files
  └── navigation.ts       # Global navigation logic

/API
  ├── app.ts
  ├── authenticationMiddleware.ts
  └── /Routes             # All route files

/Dist                      # Compiled JS files (add to .gitignore)
/node_modules              # Auto-generated (add to .gitignore)
```

---

## Development Standards

* Use **TypeScript** and ensure proper typing is followed.
* Pull requests without proper typing can be rejected.
* Ensure proper modular structure and naming conventions.
* All necessary `ReadMe.md` files must be added to relevant subdirectories for smooth onboarding and setup.

---

## Recommended Tools

* WebStorm
* Google Chrome
* MySQL Workbench
* Jira (strongly recommended for task and sprint tracking)

---

## Tech Stack

* **Liquibase**
* **TypeORM**
* **TypeScript**
* **HTML**
* **CSS**
* **MySQL**
