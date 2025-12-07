# Quickstart: Contributing to the Humanoid Robotics Book

**Input**: `plan.md`
**Output**: This guide for setting up the development environment and contributing content.

## 1. Environment Setup

To contribute to this book, you need the following installed:
-   [Node.js](https://nodejs.org/en/) (v18 or later)
-   [Yarn](https://yarnpkg.com/) (Classic or Berry)
-   [Git](https://git-scm.com/)

## 2. Project Initialization

1.  **Clone the repository**:
    ```bash
    git clone <repository-url>
    cd <repository-name>
    ```

2.  **Initialize the Docusaurus project**:
    The Docusaurus project is located in the `book/` directory.
    ```bash
    cd book
    yarn install
    ```

3.  **Run the development server**:
    ```bash
    yarn start
    ```
    This will start a local development server, typically at `http://localhost:3000`. The website will automatically reload as you edit the markdown files in `book/docs/`.

## 3. How to Write a New Section

1.  **Navigate to the `book/docs` directory**.

2.  **Open the appropriate module file** (e.g., `module-1-ros2.md`).

3.  **Add your new section** following the structure defined in the `data-model.md`. Use markdown for formatting.

    ```markdown
    ## 1.X New Section Title

    Your content here.

    ### 1.X.1 Subsection
    
    More content.
    ```

4.  **Add diagrams** by placing the image files in the `book/static/img` directory and referencing them in your markdown:
    ```markdown
    ![Alt text for image](./img/your-diagram.png)
    ```

5.  **Add citations** by following the APA 7th edition format and adding them to the "Summary & References" section of the module.

## 4. Submitting Changes

1.  **Create a new feature branch** for your changes using the `/sp.specify` command if it's a new chapter or major section. For smaller edits, a regular git branch is sufficient.

2.  **Commit your changes** with a clear commit message.
    ```bash
    git add .
    git commit -m "feat(book): add section on XYZ in Module 2"
    ```

3.  **Push your branch and open a Pull Request**.
    ```bash
    git push origin <your-branch-name>
    ```
    The PR will be reviewed for technical accuracy, clarity, and adherence to the constitution.
