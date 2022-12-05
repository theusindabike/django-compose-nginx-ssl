FROM certbot/certbot:v1.27.0

COPY certify-init.sh /opt/
RUN chmod +x /opt/certify-init.sh

# to overwrite the entrypoint
ENTRYPOINT []
CMD ["certbot", "renew"]