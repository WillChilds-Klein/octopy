FROM ubuntu

RUN apt-get update && apt-get install pip

RUN which curl || sudo apt-get install curl

RUN mkdir octopy && curl https://gist.githubusercontent.com/WillChilds-Klein/e744afb87e5221f9383e/raw/6cb9ff778932856b32dbe2eec96b3bf3e861e1ee/octo.py > octopy/octo.py

WORKDIR octopy

ENV OCTOPY_SERVER_IP 128.36.232.49

RUN python octo.py client ${OCTOPY_SERVER_IP}
