FROM python:3.6
LABEL maintainer 'Romulo Mastelari <romulo.mast@gmail.com>' 
 
RUN useradd pywww && \
    mkdir /app && \
    mkdir /log && \
    chown pywww /log
 
USER pywww
VOLUME /log
WORKDIR /app
EXPOSE 8000
 
ENTRYPOINT ["/usr/local/bin/python"]
CMD ["run.py"]