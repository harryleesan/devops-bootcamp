FROM python:2.7.14

COPY . /opt/app
WORKDIR /opt/app

RUN pip install -e .
ENV FLASK_APP flaskr
ENV FLASK_ENV development

RUN pip install '.[test]'
RUN flask init-db

CMD ["flask", "run", "--host=0.0.0.0"]

