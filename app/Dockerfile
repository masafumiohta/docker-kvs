From python:3.7.5-slim
# flaskのissueからバージョンを1.1.4にあげてかつitsdangerous==1.1.0  markupsafe==2.0.1を追記する。
RUN pip install flask==1.1.4 redis==3.3.8 itsdangerous==1.1.0  markupsafe==2.0.1
WORKDIR /src
COPY ./src/server.py /src/
ENV PORT 80
ENV DEBUG false
ENV REDIS_HOST 127.0.0.1
ENV REDIS_PORT 6379
ENV REDIS_DB 0
ENTRYPOINT ["python", "-u", "server.py"]
