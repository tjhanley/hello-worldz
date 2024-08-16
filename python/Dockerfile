# Use the official Python 3.9 image
FROM python:3.9-slim

# Set environment variables
ENV PYTHONUNBUFFERED=1

# Set work directory
WORKDIR /app

# Install Poetry
RUN pip install poetry

# Copy only pyproject.toml and poetry.lock to leverage Docker cache
COPY pyproject.toml poetry.lock /app/

# Install dependencies
RUN poetry config virtualenvs.create false && poetry install --no-dev --no-interaction --no-ansi

# Copy the rest of the application code
COPY . /app/

# Expose the port
EXPOSE 3000

# Command to run the application in reload mode
CMD ["poetry", "run", "uvicorn", "hello_world.main:app", "--host", "0.0.0.0", "--port", "3000", "--reload"]
