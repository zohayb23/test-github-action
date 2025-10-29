# Test GitHub Action Repository

This repository is used to test the **pvtr-github-repo-action** GitHub Action.

## Purpose

This repo serves as a testbed for the OSPS (Open Source Project Security) Baseline assessment action. It allows us to:

- Test the action with different configurations
- Verify the action works correctly in a real GitHub environment
- Validate the output format and results

## Usage

1. Go to the **Actions** tab in this repository
2. Select **"Test OSPS Security Assessment Action"** workflow
3. Click **"Run workflow"**
4. Configure the parameters:
   - **Target Owner**: Repository owner to assess (default: zohayb23)
   - **Target Repo**: Repository name to assess (default: test-github-action)
   - **Catalog**: OSPS catalog (default: OSPS_B)
   - **Maturity Level**: Assessment level (1, 2, or 3)
   - **Log Level**: Verbosity level (info, debug, trace)
   - **Output Format**: Results format (yaml or json)

## Expected Results

The action will:
- Analyze the target repository against OSPS Baseline controls
- Generate security assessment results
- Save results as artifacts in the workflow run
- Display a summary of findings

## Files

- `.github/workflows/test-osps-action.yml` - The test workflow file
- `evaluation_results/` - Directory where assessment results are saved (created during workflow execution)
