FROM python:3.10

# Install Java
RUN apt update && apt install -y sudo && apt install default-jdk -y

# Upgrade pip
RUN pip install --upgrade pip

# Install Jupyter Notebook
RUN pip install jupyter
RUN pip install ipykernel

# Install production dependencies
COPY requirements.txt /tmp/requirements.txt
RUN pip install -r /tmp/requirements.txt && rm /tmp/requirements.txt

# Install development dependencies
COPY requirements-dev.txt /tmp/requirements-dev.txt
RUN pip install -r /tmp/requirements-dev.txt && rm /tmp/requirements-dev.txt