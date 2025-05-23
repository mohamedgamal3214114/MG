
FROM odoo:18.0
LABEL maintainer="Mohamed Gamal"

# Copy custom addons if any
COPY ./addons /mnt/extra-addons

# Set permissions
USER root
RUN chown -R odoo:odoo /mnt/extra-addons
USER odoo

# Set default command
CMD ["odoo", "-c", "/etc/odoo/odoo.conf"]
