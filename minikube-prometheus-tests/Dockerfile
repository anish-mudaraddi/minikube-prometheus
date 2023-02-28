FROM python:3.9

# Create an Application source code directory
RUN mkdir -p /k8s_python_hello_world/src

# Set Home Directory for containers
WORKDIR /k8s_python_hello_world/src

# Install Python Dependencies
#RUN pip install --no-cahce-dir -r requirements.txt

# Copy src code to Container 
COPY app.py /k8s_python_hello_world/src/app/

# Set Application Environment variables
ENV PYTHONUNBUFFERED 1

# EXPOSE PORTS
#EXPOSE 25565

# Setup Persistent data store
#VOLUME [ "/app-data" ]

# Run Python Application
CMD ["python", "app/app.py"]