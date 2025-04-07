FROM python:3.10-slim

WORKDIR /app

# Install system dependencies
RUN apt-get update && apt-get install -y \
    build-essential git && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# Install MLflow from PyPI
RUN pip install mlflow


# Default command (can override in Kubernetes)
CMD ["tail", "-f", "/dev/null"]

