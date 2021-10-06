FROM python:3.8.0

RUN pip install git+https://github.com/harupy/mlflow@stream
RUN pip install boto3 smart_open

EXPOSE 5000

CMD mlflow server \
    --host 0.0.0.0 \
    --port 5000 \
    --default-artifact-root ${BUCKET}
