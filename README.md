# Playwright-with-pytest

### Pre-requisites:
1) Install python: https :- //www.python.org/downloads/
2) Install upgraded pip :- **pip install --upgrade pip**
3) Install the playwright python library :- **pip install playwright**
4) Install the required browsers :- **playwright install**
5) Install the Pytest plugin :- **pip install pytest-playwright**
6) Install the parallel execution plugin :- **pip install pytest-xdist**


### Libraries used:
1) **playwright** :- https://pypi.org/project/playwright/
2) **pytest-playwright** :- https://pypi.org/project/pytest-playwright/#description
3) **pytest-xdist** :- https://pypi.org/project/pytest-xdist/

### Execute Test cases: 
To run your tests, use Pytest CLI
1) Running all test cases in headless mode on Chromium :- **pytest**
2) Running all test cases in non headless mode on Chromium :- **pytest --headed**
3) Running a single test file :- **pytest test_login.py**
4) Run a set of test files :- **pytest tests/todo-page/ tests/landing-page/**
5) Run the test with the function name :- **pytest -k "test_add_a_todo_item"**
6) Running Tests on specific browsers :- **pytest test_login.py --browser webkit**
7) Running Tests on multiple browsers :- **pytest test_login.py --browser webkit --browser firefox**
8) Running Tests in parallel :- **pytest --numprocesses auto**
9) Run tests with slow mo with the --slowmo argument :- **pytest --slowmo 100**

### CLI arguments:
1) **--headed** :- Run tests in headed mode (default: headless).
2) **--browser** :- Run tests in a different browser chromium, firefox, or webkit. It can be specified multiple times (default: all browsers).
3) **--browser-channel** :- Browser channel to be used.
4) **--slowmo** :- Run tests with slow mo.
5) **--device** :- Device to be emulated.
6) **--output** :- Directory for artifacts produced by tests (default: test-results).
7) **--tracing** :- Whether to record a trace for each test. on, off, or retain-on-failure (default: off).
8) **--video** :- Whether to record video for each test. on, off, or retain-on-failure (default: off).
9) **--screenshot** :- Whether to automatically capture a screenshot after each test. on, off, or only-on-failure (default: off).

