# Debater with CrewAI

DebaterWithCrewai is a template project for building a multi-agent debate system using [crewAI](https://crewai.com). This project demonstrates how to orchestrate multiple AI agents to debate a topic, judge the arguments, and output structured results. The codebase is modular and easily extensible for your own multi-agent workflows.

---

## Tech Stack

- **Python 3.8+**: Core programming language for all logic and orchestration.
- **[crewAI](https://crewai.com)**: Framework for building and running multi-agent workflows.
- **PyYAML**: For parsing agent and task configuration files.
- **Markdown**: Output format for debate results.
- **CLI Tools**: Uses the `crewai` command-line interface for workflow execution.

Optional/Recommended:
- **uv**: Fast Python package installer (alternative to pip).
- **VSCode/Jupyter**: For code editing and experimentation.

## Features

- **Multi-Agent Debate**: Agents are assigned roles (Debater, Judge) and collaborate on a debate task.
- **Configurable Agents & Tasks**: Define agent personalities and task flows in YAML files.
- **Structured Output**: Debate results are saved to markdown files for easy review.
- **Separation of Logic**: Core logic is organized in `crew.py` and `main.py` for clarity and extensibility.

## How to Run (using crewAI CLI)

1. **Install crewAI and dependencies**  
   Make sure you have Python 3.8+ installed.  
   Install [crewAI](https://pypi.org/project/crewai/) and other dependencies:

   ```bash
   uv tool install crewai
   pip install -r requirements.txt
   ```

2. **Configure your agents and tasks**  
   Edit the YAML configuration files as needed (see `src/debater_with_crewai/crew.py` for details).

3. **Run the debate using the crewAI CLI**  
   From the project root, run:

   ```bash
   crewai run src/debater_with_crewai/crew.py
   ```

   This will launch the debate workflow using crewAI, and save the results in the `output/` directory.

4. **Review the results**  
   Open the markdown files in the `output/` folder to see the debate arguments and the judge's decision.



---

## Project Structure
