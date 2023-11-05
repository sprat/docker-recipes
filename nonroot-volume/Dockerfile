FROM alpine:latest
RUN adduser -D user && mkdir -p /app && chown user:user /app
USER user
# VOLUME /app
CMD ["/bin/sh", "-c", "echo user: $(id) -- /app: $(stat -c 'uid=%u(%U) gid=%g(%G) perm=%A' /app)"]
