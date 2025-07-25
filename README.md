# PR Preview Setup for Helm Charts

This branch sets up GitHub Actions workflows to enable previewing Helm charts for each pull request.

## Features

- ✅ Automatically packages Helm charts when a PR is opened or updated
- ✅ Publishes preview charts to the `gh-pages` branch under `preview/pr-<number>/`
- 🧹 Cleans up preview charts when the PR is closed

## How it works

1. On every PR, a `.tgz` Helm chart package is generated.
2. The chart is uploaded to the `gh-pages` branch under a path like:


