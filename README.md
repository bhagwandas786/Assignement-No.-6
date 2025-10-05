# GitHub Actions CI/CD Assignment - 06

This repository demonstrates the implementation of two automated CI/CD pipelines using GitHub Actions. The project fulfills the assignment requirements of creating workflows that execute shell scripts and run linting and testing operations.

## 📋 Assignment Overview

This repository implements two automated CI/CD workflows as per assignment requirements:
- **Workflow 1**: Executes a shell script on push and pull request events
- **Workflow 2**: Runs linting and testing operations on code changes

## 🏗️ Repository Structure
*github-actions-assignment/*

├── .github/
│ └── workflows/
│ ├── run-script.yml # Shell script execution workflow
│ └── lint-test.yml # Linting and testing workflow
├── math.js # Utility functions module
├── test.js # Test cases implementation
├── package-locke # exact versions of dependencies
├── run.sh # Demonstration shell script
├── package.json # Project configuration
└── README.md # Documentation


## ⚙️ Workflows

### 1. Shell Script Execution
**File**: `.github/workflows/run-script.yml`
- Triggers on: `push` and `pull_request` events
- Executes: `run.sh` script
- Environment: Ubuntu latest

### 2. Linting and Testing  
**File**: `.github/workflows/lint-test.yml`
- Triggers on: `push` and `pull_request` events
- Runs: `npm run lint` and `npm test`
- cache: npm 
- Environment: Node.js 18 on Ubuntu

## 📊 Implementation Details

### Files
```bash
#run.sh

#!/bin/bash
echo "Hello World from Bhagwan and Sir"
#package.json

json
{
  "name": "github-actions-assignment",
  "version": "1.0.0",
  "scripts": {
    "lint": "echo 'Linting code...'",
    "test": "node test.js"
  }
}

#Source Files

math.js: Contains utility functions (add, subtract)
test.js: Implements test cases for verification

🚀 Usage

Automatic Execution: Workflows run automatically on push/PR events
Manual Trigger: Navigate to Actions tab → Select workflow → Run workflow
Results: Check GitHub Actions tab for execution logs and results

📈 Results Verification

✅ Green checkmark indicates successful execution
❌ Red cross indicates failure with detailed logs
⏱️ Real-time execution monitoring available.
