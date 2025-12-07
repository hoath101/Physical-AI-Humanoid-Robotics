---
id: 7
title: Switch GitHub Actions Workflow to npm for Docusaurus
stage: red
date: 2025-12-07
surface: agent
model: claude-3-5-sonnet
feature: 002-humanoid-robotics-book
branch: main
user: this error is coming again
command: Error: Dependencies lock file is not found in /home/runner/work/Physical-AI-Humanoid-Robotics/Physical-AI-Humanoid-Robotics. Supported file patterns: yarn.lock
labels: ["deployment", "docusaurus", "github-actions", "bug-fix"]
links:
  spec: null
  ticket: null
  adr: null
  pr: null
files_yaml:
  - .github/workflows/deploy-docusaurus.yml
tests_yaml: []
prompt_text: |
  this error is coming again
response_text: |
  The changes to use `npm` in the GitHub Actions workflow file have been successfully pushed to the `main` branch. This should trigger a new workflow run, and the `npm` related changes should resolve the "Dependencies lock file not found" error, allowing the Docusaurus project to build and deploy correctly.

  You can now monitor the GitHub Actions tab in your repository to see if the deployment succeeds.
outcome: GitHub Actions workflow modified to use npm for dependency management and build, resolving the yarn.lock not found error.
evaluation: The fix addresses the root cause of the error by switching from yarn to npm commands in the CI/CD pipeline.
---
