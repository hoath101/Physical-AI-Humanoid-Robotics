---
id: 6
title: Fix GitHub Actions Workflow for Docusaurus Lock File
stage: red
date: 2025-12-07
surface: agent
model: claude-3-5-sonnet
feature: 002-humanoid-robotics-book
branch: main
user: Error: Dependencies lock file is not found in /home/runner/work/Physical-AI-Humanoid-Robotics/Physical-AI-Humanoid-Robotics. Supported file patterns: yarn.lock
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
  Error: Dependencies lock file is not found in /home/runner/work/Physical-AI-Humanoid-Robotics/Physical-AI-Humanoid-Robotics. Supported file patterns: yarn.lock
response_text: |
  The changes to the GitHub Actions workflow file have been successfully pushed to the `main` branch. This should trigger a new workflow run, and the `working-directory` fix should resolve the "Dependencies lock file not found" error.

  You can now monitor the GitHub Actions tab in your repository to see if the deployment succeeds.
outcome: GitHub Actions workflow modified to correctly locate yarn.lock by adding working-directory.
evaluation: The fix addresses the reported error by adjusting the working directory for yarn commands in the CI/CD pipeline.
---
