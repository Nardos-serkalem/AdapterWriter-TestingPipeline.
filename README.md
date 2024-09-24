# Adapters and Writers Test Workflow

This repository contains a GitHub Actions workflow for managing and testing changes in adapters and writers within the Biocypher Metta project.

## Features

- Automated Testing: Triggers on changes to adapters, writers, configuration files, and the main script.
- Change Detection: Identifies and categorizes changes in files.
- Prioritized Testing:
  - If both writer and config change, all adapter tests are run.
  - If only the config changes, tests run based on the specific config changes.
  - If only the writer changes, all adapter tests are executed.

