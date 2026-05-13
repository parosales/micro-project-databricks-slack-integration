# micro-project-data-profiling-with-claude

Micro-project to integrate the Databricks Free Environment with Slack (the communications App).


# 1. Overview

## 1.1. Goals

### 1.1.1. General Goal

To understand how to integrate the Databricks Free Environment with Slack (the communications App).

### 1.1.2. Specific Goals

1. To integrate the Databricks Free Environment with Slack.
2. To use the integration to alert on the executions and status of a sample job that runs a notebook scheduled in Databricks.

### 1.1.3. Problem Definition

#### Part 1:  Integration of Slack with Databricks Free Edition.

Slack is a widely used communication platform that can be integrated with various tools and services. The integration of Slack with Databricks Free Edition will allow users to receive notifications and alerts about the status of their Databricks jobs and workloads.

#### Part 2:  Alerts on Job Execution

To validate the integration, a sample job will be created and scheduled to run a notebook. The integration will be used to alert on the executions and status of the job.

# 2. Requirements

### 2.1. User Requirements

- Alerts on job execution status (success, failure, etc.) are delivered to a Slack channel, in Slack desktop and mobile.

## 2.2. System Requirements

### 2.2.1. Slack Integration with Databricks Free.

- The integration must allow Slack to access jobs execution status in Databricks.
- The integration must be documented and reproducible.
- Databricks must notify Slack on job execution status.
 
### 2.2.2. Toolkit 

- Running environment:  Databricks Free Edition.
- Programming Language:  Python
- Data frameworks:  PySpark
- IDE:  Windsurf
- Code Versioning System:  git + GitHub
- Databricks notebook.
- Agents to use:  Main:  Claude Code;  Secondary:  Genie Code
- Communication Tool:  Slack desktop and mobile

### 2.2.3. Job to run

- Any, as long as it can be scheduled and executed in Databricks Free Edition.

### 2.3. Non-functional requirements

### 2.3.1. System Components

- Notebook that executes a simple job
- Databricks scheduled Job

### 2.3.2. Other deliverables

- Prompts used to instruct the LLM
- Claude code configuration files:  claude.md, commands
- Updated repository in Git
- Lessons Learned:  documented as part of this README.md file

### 2.3.3. Approach

- Approach to use LLMs:  high-level instructions, best pratices used in Claude Code.  Avoid micro-managing the LLM.

## 2.4. Scope

N/a

## 2.5. Assumptions

n/a

# 3. Lessons and Conclusions

## 3.1. Lessons Learned

TBD

## 3.2. Conclusions

TBD

# Appendixes

## Appendix 1:  Future Work

## Appendix 2: References

