FROM python:3.9.6


# create root directory for our project in the container
WORKDIR /api
#Copy project and dependencies
COPY . .
RUN pip install --upgrade pip && pip install -r requirements.txt

EXPOSE 8000

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

