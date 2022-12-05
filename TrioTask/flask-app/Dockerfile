#Use Python 3.6 as a base image
FROM python:3.7
WORKDIR /PROGVER/trio-task/flask-app
# Copy contents into image
COPY app.py .
COPY requirements.txt .
 
# install pip dependencies from requirements file
RUN pip install Flask
RUN pip install -r requirements.txt
 
# Expose correct port
EXPOSE 5000
# Create an entrypoint
ENTRYPOINT ["python", "app.py", "requirements.txt"]
