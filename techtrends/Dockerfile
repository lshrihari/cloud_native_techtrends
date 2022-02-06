FROM python:3.8

LABEL maintainer="Shrihari Vasudevan"

RUN adduser --disabled-password --gecos "" appuser
USER appuser
WORKDIR /home/appuser
ENV PATH='/home/appuser/.local/bin':$PATH

COPY --chown=appuser:appuser . /home/appuser
RUN pip install --user -r requirements.txt
RUN python init_db.py

EXPOSE 3111
CMD ["python", "app.py"]


