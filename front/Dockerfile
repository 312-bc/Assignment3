FROM python:3.6
EXPOSE 3001
WORKDIR /app
COPY requirements.txt .
ADD front.py .
RUN pip install -r requirements.txt
ADD . /templates
WORKDIR /app/templates
COPY templates/layout.html .
COPY templates/index.html .
WORKDIR /app
CMD python ./front.py
