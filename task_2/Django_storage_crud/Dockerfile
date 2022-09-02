FROM python:3.10

COPY ./requirements.txt /src/requirements.txt

RUN pip install --no-cache-dir --upgrade -r /src/requirements.txt

WORKDIR /src

COPY . /src

EXPOSE 8000

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]