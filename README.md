# GITWITHGPT
This repository demonstrates an automated GitHub workflow that uses **OpenAI’s GPT** to process changes in your codebase and create a pull request with generated summaries or transformations.

## How It Works

1. **GitHub Action triggers** on each push to `main` (configurable).
2. It **determines which files have changed** by comparing the latest commit to the previous one.
3. A **Python script** (`scripts/gpt_processor.py`) uses OpenAI’s GPT API to process or summarize the changed files.
4. If the script produces a new or updated file (`GPT_SUMMARY.md`), the Action **commits** those changes to a branch named `gpt-automatic-updates`.
5. The Action then **opens a pull request** from `gpt-automatic-updates` to `main`, letting you review or merge the automated output.

# Fault Detection and Specification Analysis in Business Process Logic Systems Using LLMs

## Overview

This repository provides an automated framework for analyzing and improving business process logic systems using Large Language Models (LLMs). The system has two primary components:

1. **Specification Analysis**: Identifies missing or redundant specifications and suggests improvements.
2. **Fault Detection in BPMN Files**: Detects logical and structural faults in BPMN workflows and applies corrections.

### Key Features

- **Specification Analysis:** Uses clustering and semantic embeddings to analyze discrepancies in specifications.
- **Fault Detection:** Identifies BPMN-specific errors such as missing decision gateways and incorrect links.
- **LLM Integration:** Leverages the Ollama Mistral and OpenAI GPT-4o models for generating improvement suggestions and BPMN corrections.
- **Automated Correction:** Applies AI-driven improvements to both textual specifications and BPMN XML files.

## License

This project is licensed under the MIT License.

