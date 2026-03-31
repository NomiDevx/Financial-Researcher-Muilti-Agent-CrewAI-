# FinancialResearcher CrewAI Financial Market Analysis System

This project implements a multi-agent AI workflow designed to analyze financial markets and generate professional investment reports. It leverages specialized AI agents to simulate real-world financial research and reporting processes.

🚀 Overview

The system consists of two collaborative AI agents:

Financial Researcher
Financial Reporting Analyst

Together, they:

Analyze current market trends
Identify high-potential stocks
Generate structured investment reports
🧠 Agents
🔍 Financial Researcher

Role: Financial Researcher
Model: deepseek/deepseek-chat

Responsibilities:

Analyze current financial markets using available data
Research latest news, trends, and stock fundamentals
Identify top-performing and high-growth stocks
Focus on uncovering undervalued or high-potential opportunities

Expertise:

10+ years of market experience
Strong in trend analysis and stock evaluation
Data-driven decision making
📝 Financial Reporting Analyst

Role: Financial Reporting Analyst
Model: deepseek/deepseek-chat

Responsibilities:

Convert raw research into structured reports
Present findings in a clear, professional format
Ensure readability and actionable insights
Summarize key investment opportunities

Expertise:

Financial reporting and documentation
Data synthesis and presentation
Business-level communication
📌 Tasks
📈 Financial Research Task

Objective:
Identify the top 5 stocks to invest in right now based on:

Market trends
Recent news
Fundamental analysis
Growth potential

Output:

Stock name & ticker
Market context
Investment rationale
📊 Reporting Task

Objective:
Transform research findings into a comprehensive investment report.

Output:

Clean markdown report
Investment thesis for each stock
Summary of current market conditions
Easy-to-read structured format
⚙️ Workflow
Financial Researcher gathers and analyzes market data
Selects top 5 stock opportunities
Reporting Analyst processes findings
Generates a polished investment report
🧩 Tech Stack
LLM: DeepSeek Chat (deepseek/deepseek-chat)
Framework: CrewAI (or similar multi-agent orchestration)
Language: Python

## Installation

Ensure you have Python >=3.10 <3.14 installed on your system. This project uses [UV](https://docs.astral.sh/uv/) for dependency management and package handling, offering a seamless setup and execution experience.

First, if you haven't already, install uv:

```bash
pip install uv
```

Next, navigate to your project directory and install the dependencies:

(Optional) Lock the dependencies and install them by using the CLI command:
```bash
crewai install
```
### Customizing

**Add your `OPENAI_API_KEY` into the `.env` file**

- Modify `src/financial_researcher/config/agents.yaml` to define your agents
- Modify `src/financial_researcher/config/tasks.yaml` to define your tasks
- Modify `src/financial_researcher/crew.py` to add your own logic, tools and specific args
- Modify `src/financial_researcher/main.py` to add custom inputs for your agents and tasks

## Running the Project

To kickstart your crew of AI agents and begin task execution, run this from the root folder of your project:

```bash
$ crewai run
```

This command initializes the financial_researcher Crew, assembling the agents and assigning them tasks as defined in your configuration.

This example, unmodified, will run the create a `report.md` file with the output of a research on LLMs in the root folder.

## Understanding Your Crew

The financial_researcher Crew is composed of multiple AI agents, each with unique roles, goals, and tools. These agents collaborate on a series of tasks, defined in `config/tasks.yaml`, leveraging their collective skills to achieve complex objectives. The `config/agents.yaml` file outlines the capabilities and configurations of each agent in your crew.

## Support

For support, questions, or feedback regarding the FinancialResearcher Crew or crewAI.
- Visit our [documentation](https://docs.crewai.com)
- Reach out to us through our [GitHub repository](https://github.com/joaomdmoura/crewai)
- [Join our Discord](https://discord.com/invite/X4JWnZnxPb)
- [Chat with our docs](https://chatg.pt/DWjSBZn)

Let's create wonders together with the power and simplicity of crewAI.
