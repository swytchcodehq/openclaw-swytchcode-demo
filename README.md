# OpenClaw + Swytchcode GitHub Issue Triage Bot

Demonstrates OpenClaw (AI agent) using Swytchcode CLI as the execution layer to triage GitHub issues.

## Setup

1. Install swytchcode: `npm install -g swytchcode@latest`
2. `swytchcode init --editor=none --mode=sandbox --non-interactive`
3. `swytchcode get github`
4. `swytchcode add repos.issue.get`
5. `swytchcode add repos.issue.comments.create`

## Run
$env:GITHUB_TOKEN="your_pat"
$env:GITHUB_OWNER="lakshayom2015"
$env:GITHUB_REPO="stripe-integration-test"
go run .

## Stack
- AI Agent: OpenClaw (openclaw.ai)
- Execution Layer: Swytchcode CLI v2.2.7 (cli.swytchcode.com)
- GitHub Integration: github.github@1.1.4
- Language: Go (stdlib only, no external dependencies)
