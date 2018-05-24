FROM cloudfoundry/cflinuxfs2

COPY bbr /usr/bin/bbr

RUN chmod +x /usr/bin/bbr

# Verify image
COPY verify_image.sh /tmp/verify_image.sh
RUN /tmp/verify_image.sh && rm /tmp/verify_image.sh
