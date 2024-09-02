FROM python:3.9-slim

WORKDIR /data

# Install Django
RUN pip install django==3.2

# Copy the application code to the container
COPY . .

# Run Django migrations
RUN python manage.py migrate

# Expose the application port
EXPOSE 8000

# Start the Django development server
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]


