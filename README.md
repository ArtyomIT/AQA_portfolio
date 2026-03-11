# Playwright Test Framework

UI test automation framework built with **Python**, **Pytest** and **Playwright**.

## About

This project demonstrates a structured approach to web UI testing using the **Page Object Model**.

It covers core automation practices such as:

- page object architecture
- reusable pytest fixtures
- parametrized tests
- positive and negative scenarios
- smoke and regression suites
- UI validation with Playwright assertions
- configurable test environment via `pytest.ini`
- clean and readable test structure for scaling

The framework uses **SauceDemo** as the target application for testing typical e-commerce flows such as login, inventory interactions, cart operations, sorting, and checkout.

## Tech Stack

- Python
- Pytest
- Playwright
- pytest-playwright

## Setup
```bash
# Clone repository
git clone https://github.com/ArtyomIT/playwright-test-framework.git
cd playwright-test-framework

# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Install Playwright browsers:
playwright install
```

## Run Tests
```bash
# Run all tests:
pytest

# Run smoke tests:
pytest -m smoke

# Run regression tests:
pytest -m regression

# Run only authorization tests:
pytest -m auth

# Run only positive scenarios:
pytest -m positive

# Run only negative scenarios:
pytest -m negative

# Run tests in headed mode:
pytest --headed
```

## Goal

This repository was created as part of my QA Automation portfolio to demonstrate practical skills in:

- UI test automation with Playwright

- test framework design with Pytest

- building maintainable Page Object architecture

- writing clear and scalable automated test scenarios
