# Learning to destroy secrets

Sometimes we do some mistakes and commit secrets to our repositories. This is a simple guide to help you destroy secrets from your git history.

## Step 1: Identify the secrets

First of all, you need to identify the secrets that you want to destroy. This can be passwords, API keys, tokens, etc.

## Step 2: Remove the secrets

After identifying the secrets, you need to remove them from your code. This can be done by replacing the secrets with dummy values or by removing them completely.

```bash

git filter-repo --invert-paths --path 'secrets.txt'

# or if didn't work add --force

```

This will clear up all the commits where this file existed.

## Step 3: Setup the required environment with new variables and a new commit
