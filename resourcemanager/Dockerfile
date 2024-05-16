FROM sevenrats/hadoop-base:latest

LABEL org.opencontainers.image.authors="austin@crandall.codes"

HEALTHCHECK CMD curl -f http://localhost:8088/ || exit 1

ADD entrypoint.sh /entrypoint.sh
RUN chmod a+x /entrypoint.sh

EXPOSE 8088

CMD ["/entrypoint.sh"]
