# Data Model: Humanoid Robotics Book

**Input**: `plan.md`
**Output**: This document, describing the logical structure of the book content.

## Entity Relationship Diagram (Logical)

```
Book
 │
 ├── Module 1
 │     ├── Section 1.1 (Intro)
 │     ├── Section 1.2 (Core Concepts)
 │     │     └── Subsection 1.2.1
 │     ├── Section 1.3 (Tools & Frameworks)
 │     ├── Section 1.4 (Applied Workflow)
 │     ├── Section 1.5 (Mini Project)
 │     └── Section 1.6 (Summary & References)
 │
 ├── Module 2
 │     └── ... (same section structure)
 │
 ├── Module 3
 │     └── ... (same section structure)
 │
 └── Module 4
       └── ... (same section structure)
```

## Entity Definitions

### Book

The top-level entity, representing the entire collection of modules.

-   **Attributes**:
    -   `title`: The main title of the book.
    -   `author`: The author(s) of the book.
    -   `version`: The semantic version of the book.

### Module

A major part of the book, focused on a specific high-level topic (e.g., ROS 2, Digital Twin).

-   **Attributes**:
    -   `module_number`: The sequential number of the module (1, 2, 3, 4).
    -   `title`: The title of the module.
-   **Relationships**:
    -   Belongs to one `Book`.
    -   Has many `Sections`.

### Section

A self-contained chapter within a module.

-   **Attributes**:
    -   `section_number`: The sequential number of the section within the module (e.g., 1.1, 1.2).
    -   `title`: The title of the section (e.g., "Introduction", "Core Concepts").
    -   `content`: The markdown content of the section.
-   **Relationships**:
    -   Belongs to one `Module`.
    -   Can have many `Subsections`.

### Subsection

A smaller part within a section, used for breaking down complex topics.

-   **Attributes**:
    -   `subsection_number`: The sequential number of the subsection (e.g., 1.2.1).
    -   `title`: The title of the subsection.
    -   `content`: The markdown content of the subsection.
-   **Relationships**:
    -   Belongs to one `Section`.

## Validation Rules

-   Each `Module` must contain all standard `Sections` as defined in the constitution: Introduction, Core Concepts, Tools & Frameworks, Applied Workflow, Mini Project, and Summary & References.
-   `section_number` and `subsection_number` must be unique within their parent entity.
-   All `content` must be valid Markdown.
