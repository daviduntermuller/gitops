FROM python:3.8.2

RUN mkdir /app
COPY Pipfile /app/
COPY main.py /app/
WORKDIR /app
RUN pip install --upgrade pip && pip install pipenv && pipenv install

EXPOSE 5000
CMD ["pipenv", "run", "python", "/app/main.py"]% 
