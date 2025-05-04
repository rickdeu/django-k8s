FROM python:3.13.2-slim	

COPY . /app

WORKDIR /app

RUN python3 -m venv venv /opt/venv

RUN /opt/venv/bin/pip install pip --upgrade && \
     /opt/venv/bin/pip  install -r requirements.txt &&  \
     chmod +x /app/entrypoint.sh && chmod +x /app/migrate.sh

     

CMD [ "/app/entrypoint.sh"]











