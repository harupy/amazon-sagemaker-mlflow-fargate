FROM python:3.8.0

RUN echo bar
RUN pip install git+https://github.com/harupy/mlflow.git@stream
RUN pip install boto3 smart_open

EXPOSE 5000

CMD mlflow server \
    --host 0.0.0.0 \
    --port 5000 \
    --default-artifact-root ${BUCKET}
