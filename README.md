# GITWITHGPT
This repository demonstrates an automated GitHub workflow that uses **OpenAI’s GPT** to process changes in your codebase and create a pull request with generated summaries or transformations.

## How It Works

1. **GitHub Action triggers** on each push to `main` (configurable).
2. It **determines which files have changed** by comparing the latest commit to the previous one.
3. A **Python script** (`scripts/gpt_processor.py`) uses OpenAI’s GPT API to process or summarize the changed files.
4. If the script produces a new or updated file (`GPT_SUMMARY.md`), the Action **commits** those changes to a branch named `gpt-automatic-updates`.
5. The Action then **opens a pull request** from `gpt-automatic-updates` to `main`, letting you review or merge the automated output.

## License

This project is licensed under the MIT License.

