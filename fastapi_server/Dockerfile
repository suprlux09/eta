FROM python:3.10
WORKDIR /app
COPY ./requirements.txt /app/requirements.txt
RUN pip3 install -r requirements.txt
COPY . /app
ENV ETA_OPENAI_KEY=$ETA_OPENAI_KEY
EXPOSE 8000
ENTRYPOINT ["python3", "main.py"]