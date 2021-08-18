FROM alpine
ADD  ./server.sh /server.sh
RUN apk update \
  && apk add netcat-openbsd \
  && chmod +x /server.sh
EXPOSE 1234
CMD /server.sh
