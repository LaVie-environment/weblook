FROM busybox
COPY watcher.sh /watcher
WORKDIR da_agent

RUN adduser -DHs /bin/bash example
RUN chown example watcher.sh
RUN chmod a+x watcher.sh
USER example

CMD ["./watcher.sh"]