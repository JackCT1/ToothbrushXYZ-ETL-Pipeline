FROM public.ecr.aws/lambda/python:3.8

COPY ingestion_script.py ${LAMBDA_TASK_ROOT}

COPY requirements.txt .

RUN pip3 install -r requirements.txt --target "${LAMBDA_TASK_ROOT}"

CMD ["ingestion_script.handler"]