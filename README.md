# Assignment 2: ReAct Agent

A ReAct (Reason + Act) agent built with the Google Gemini API in Google Colab.

## What it does
The agent reads a question, decides whether it needs to search, calls a
`search_documents` tool over a small collection of cooking documents, reads the
result, and then gives a final answer.

## How it works
1. The user asks a question.
2. The model decides to call the search tool.
3. The tool returns the most relevant documents.
4. The model reads the result and answers.
5. If the documents don't contain the answer, the agent says so and uses general knowledge.

## Files
- `agent_loop_demo.ipynb`: the Colab notebook with the full agent and test questions

## How to run
1. Open the notebook in Google Colab.
2. Add your Gemini API key to Colab Secrets with the name `GOOGLE_API_KEY`.
3. Run all cells.

