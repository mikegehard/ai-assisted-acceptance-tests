# PlaywrightFlowGen: AI-Generated Playwright Test Tool

## 1. Executive Summary

PlaywrightFlowGen is an open-source CLI tool that automatically generates Playwright-based acceptance tests by using AI to discover and analyze user flows in web applications. It addresses the significant pain point of browser-based acceptance tests being too expensive and time-consuming to write and maintain manually, which often leads to inadequate test coverage and reduced confidence when making code changes.

## 2. System Overview

### 2.1 Core Workflow

1. Developer runs the tool against a target website (development/staging environment)
2. Tool automatically crawls the site and discovers possible user flows
3. Tool provides descriptions of each discovered flow
4. Developer selects important flows to test
5. Tool generates Playwright tests implementing best practices
6. Tool validates the generated tests against the target environment

### 2.2 Value Proposition

This tool enables developers to quickly generate comprehensive, maintainable Playwright tests without the traditional effort required, increasing test coverage and providing confidence when refactoring or modifying existing code.

## 3. Goals

PlaywrightFlowGen addresses the critical need for automated acceptance test generation, reducing the barrier to implementing comprehensive test coverage for web applications. By leveraging AI to analyze user flows and generate high-quality Playwright tests, this tool empowers developers to make changes with confidence, knowing that critical user-facing functionality is being tested.

## 4. Running the Project

### 4.1 Prerequisites

- Python 3.13.x
- UV package manager

### 4.2 Running the Application

To run the main application:

```bash
uv run src/main.py
```

### 4.3 Running with Arguments

If you need to pass arguments to the application:

```bash
uv run src/main.py arg1 arg2
```

### 4.4 Running Modules

To run a specific module:

```bash
uv run -m module_name
```

No virtual environment activation is required as UV handles dependencies automatically.