FROM python:3.12-slim-bookworm

ENV LANG=C.UTF-8
ENV LC_ALL=C.UTF-8

RUN apt-get update && apt-get install -y p7zip-full git && pip install PyGithub

ADD release_zips.py /release_zips.py

ENTRYPOINT ["python", "/release_zips.py"]
