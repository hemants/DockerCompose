FROM oraclelinux:8-slim

RUN microdnf install oracle-instantclient-release-el8 && \
microdnf install oracle-instantclient-basic oracle-instantclient-devel oracle-instantclient-sqlplus && \
microdnf install -y python3 && \
microdnf clean all && \
curl -O https://bootstrap.pypa.io/get-pip.py && python3 get-pip.py && pip install awscli --upgrade

CMD ["sqlplus", "-v"]
