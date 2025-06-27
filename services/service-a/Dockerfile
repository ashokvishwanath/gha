FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Copy the app
COPY app.py .

# Install dependencies
RUN pip install flask

# Expose port and run the app
EXPOSE 5000
CMD ["python", "app.py"]
