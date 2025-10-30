FROM public.ecr.aws/lambda/python:3.13

COPY handler.py ${LAMBDA_TASK_ROOT}/

RUN pip install --no-cache-dir pillow boto3 -t ${LAMBDA_TASK_ROOT}

# Lambda entrypoint
CMD ["handler.resize_handler"]