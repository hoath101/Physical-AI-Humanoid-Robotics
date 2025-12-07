# Tasks: Humanoid Robotics Book

**Input**: Design documents from `/specs/002-humanoid-robotics-book/`
**Prerequisites**: plan.md, spec.md

## Phase 1: Setup

**Purpose**: Project initialization for the Docusaurus book.

- [X] T001 Initialize a new Docusaurus project in the `book/` directory.
- [X] T002 [P] Configure basic Docusaurus settings in `book/docusaurus.config.js` (project title, theme, etc.).

---

## Phase 2: Foundational (Blocking Prerequisites)

**Purpose**: Core structure for the book content.

- [X] T003 Create placeholder markdown files for each module in `book/docs/`: `module-1-ros2.md`, `module-2-digital-twin.md`, `module-3-isaac.md`, `module-4-vla.md`.
- [X] T004 Configure the sidebar navigation in `book/docusaurus.config.js` to create a logical flow for the 4 modules.
- [X] T005 Define and document a standard markdown template for module content that includes all required sections (Intro, Concepts, Tools, Workflow, Project, Summary/References).

---

## Phase 3: User Story 1 - Write Module 1 (ROS 2) (Priority: P1) 🎯 MVP

**Goal**: Complete the full draft of the first module on ROS 2.

**Independent Test**: The `module-1-ros2.md` file is fully populated, and the Docusaurus site builds successfully with the new content.

- [X] T006 [US1] Write content for the "Introduction" section of `book/docs/module-1-ros2.md`.
- [X] T007 [US1] Write content for the "Core Concepts" section of `book/docs/module-1-ros2.md`.
- [X] T008 [P] [US1] Create diagrams for ROS 2 concepts (e.g., ROS graph) and save them to `book/static/img/`.
- [X] T009 [US1] Write content for the "Tools & Frameworks" section of `book/docs/module-1-ros2.md`.
- [X] T010 [US1] Write content for the "Applied Workflow" section, providing step-by-step examples, in `book/docs/module-1-ros2.md`.
- [X] T011 [US1] Write content for the "Mini Project" section of `book/docs/module-1-ros2.md`.
- [X] T012 [US1] Write content for the "Summary & References" section, ensuring all citations are in APA 7th format, in `book/docs/module-1-ros2.md`.

---

## Phase 4: User Story 2 - Write Module 2 (Digital Twin) (Priority: P2)

**Goal**: Complete the full draft of the second module on Simulation.

**Independent Test**: The `module-2-digital-twin.md` file is fully populated.

- [X] T013 [US2] Write content for all sections of `book/docs/module-2-digital-twin.md`, following the standard template.
- [X] T014 [P] [US2] Create diagrams for simulation concepts (e.g., sensor simulation) and save them to `book/static/img/`.

---

## Phase 5: User Story 3 - Write Module 3 (NVIDIA Isaac) (Priority: P3)

**Goal**: Complete the full draft of the third module on NVIDIA Isaac.

**Independent Test**: The `module-3-isaac.md` file is fully populated.

- [X] T015 [US3] Write content for all sections of `book/docs/module-3-isaac.md`, following the standard template.
- [X] T016 [P] [US3] Create diagrams for Isaac-specific concepts (e.g., VSLAM pipeline) and save them to `book/static/img/`.

---

## Phase 6: User Story 4 - Write Module 4 (VLA) (Priority: P4)

**Goal**: Complete the full draft of the fourth module on Vision-Language-Action.

**Independent Test**: The `module-4-vla.md` file is fully populated.

- [X] T017 [US4] Write content for all sections of `book/docs/module-4-vla.md`, following the standard template.
- [X] T018 [P] [US4] Create diagrams for VLA concepts and save them to `book/static/img/`.

---

## Phase 7: Polish & Cross-Cutting Concerns

**Purpose**: Finalize the book for publication.

- [X] T019 [P] Create a glossary of all technical terms and add it as a new page in `book/docs/`.
- [X] T020 Review all modules for consistency and add cross-links between related topics.
- [X] T021 Run a full grammar and spell check on all markdown files.
- [X] T022 Manually validate all code examples and mini-projects for reproducibility.
- [X] T023 Build the Docusaurus site locally (`yarn build`) and test for broken links or formatting issues.
- [X] T024 Configure a GitHub Actions workflow in `.github/workflows/` to automatically build and deploy the Docusaurus site to GitHub Pages on push to `main`.
- [X] T025 Document the key decisions from `research.md` as ADRs in the `history/adr/` directory.

---

## Dependencies & Execution Order

- **Setup & Foundational (Phases 1-2)**: Must be completed before any module writing begins.
- **User Stories (Phases 3-6)**: Can be worked on in parallel by different writers, but should be completed in priority order if done by a single writer.
- **Polish (Phase 7)**: Depends on all user story phases being complete.