FROM public.ecr.aws/lambda/python:3.10
WORKDIR ${LAMBDA_TASK_ROOT}

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt -t ./vendored

COPY app.py 

CMD [ "handler.handler" ]

