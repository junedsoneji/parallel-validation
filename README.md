# Parallel Validation

A simple GitHub Actions project demonstrating how to run multiple CI jobs in parallel.

## Overview

This repository contains a GitHub Actions workflow named `parallel-check` that runs frontend and backend validation jobs simultaneously whenever changes are pushed to the `main` branch.

## Workflow Details

Workflow file: `.github/workflows/parallel-check.yml`

The workflow includes two independent jobs:

- **frontend-check** — Prints a frontend validation message.
- **backend-check** — Prints a backend validation message.

Both jobs run on `ubuntu-latest` and execute independently in parallel.

## Trigger

The workflow runs automatically on every push to the `main` branch.

## Expected Result

Both jobs should complete successfully:

- Frontend validation: Success
- Backend validation: Success
- Overall workflow: Success

## Technologies

- Git and GitHub
- GitHub Actions
- Ubuntu GitHub-hosted runners
- YAML

## Purpose

This project demonstrates GitHub Actions workflow configuration, parallel job execution, and continuous integration basics.
