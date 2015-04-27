FROM ubuntu

RUN apt-get update && apt-get install pip

RUN which curl || sudo apt-get install curl

RUN mkdir octopy && cd octopy && curl https://gist.githubusercontent.com/WillChilds-Klein/e744afb87e5221f9383e/raw/6cb9ff778932856b32dbe2eec96b3bf3e861e1ee/octo.py > octo.py

ENV OCTOPY_SERVER_IP 127.0.0.1

RUN python octo.py client ${OCTOPY_SERVER_IP}
