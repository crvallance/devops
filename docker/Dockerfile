FROM python:3.8-slim
WORKDIR /mycode
RUN apt-get update && apt-get install git -y
RUN pip install uvicorn fastapi
RUN git clone https://github.com/crvallance/devops.git
WORKDIR devops/service
EXPOSE 8000
CMD uvicorn --host 0.0.0.0 demo:app