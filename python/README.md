# Hello World FastAPI

A simple "Hello, World!" RESTful API using FastAPI.

## Getting Started

These instructions will help you set up and run the project on your local machine.

### Prerequisites

- [Python 3.9+](https://www.python.org/)
- [Poetry](https://python-poetry.org/)

### Installation

1. Clone the repository or download the project files.

2. Navigate to the project directory:

   ```bash
   cd path/to/your/project
   ```

3. Install the dependencies:

   ```bash
   poetry install
   ```

4. Running the Application

To start the application, run:

    ```bash
    poetry run uvicorn hello_world.main:app --reload
    ```
