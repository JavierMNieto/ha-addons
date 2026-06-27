FROM ghcr.io/warreth/gphotos2immich:latest

ARG BUILD_ARCH
ARG BUILD_VERSION
LABEL \
  io.hass.type="addon" \
  io.hass.arch="${BUILD_ARCH}" \
  io.hass.version="${BUILD_VERSION}"

ENV PORT=8383
RUN rm -rf /app/data /app/config.json \
 && ln -s /data/cache       /app/data \
 && ln -s /data/config.json /app/config.json
