FROM cloudfoundry/cflinuxfs2

COPY bbr /usr/bin/bbr
COPY om /usr/bin/om

RUN chmod +x /usr/bin/bbr
RUN chmod +x /usr/bin/om
RUN sync

# Verify image
COPY verify_image.sh /tmp/verify_image.sh
RUN /tmp/verify_image.sh && rm /tmp/verify_image.sh
