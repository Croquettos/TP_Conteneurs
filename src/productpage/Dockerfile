FROM python:3.7.7
WORKDIR /opt/microservices
COPY productpage.py requirements.txt test-requirements.txt ./
COPY static ./static
COPY templates ./templates
COPY tests ./tests
RUN ["pip", "install", "--no-cache-dir", "-r", "requirements.txt"]
ARG FLOOD_FACTOR_TEMP=0
ENV FLOOD_FACTOR=$FLOOD_FACTOR_TEMP
EXPOSE 9080
CMD ["python", "productpage.py", "9080"]