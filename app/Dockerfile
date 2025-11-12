# Use an official Python runtime as the base image
FROM python:3.11-slim

# Set the working directory inside the container
WORKDIR /app

# Copy everything from app/ folder to /app in the container
COPY . /app

# Install dependencies (example uses FastAPI and Uvicorn)
RUN pip install --no-cache-dir fastapi uvicorn

# Expose the application port
EXPOSE 8000

# Start the FastAPI app when container runs
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]

