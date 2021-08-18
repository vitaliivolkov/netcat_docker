FROM alpine
ADD  ./client.sh /client.sh
RUN apk update \
  && apk add netcat-openbsd \
  && chmod +x /client.sh
EXPOSE 1234
CMD /client.sh
