FROM --platform=linux/arm64 torizon/chromium:3

USER root

RUN apt-get -y update \
    && apt-get install -y --no-install-recommends \
    libasound2 \
    alsa-utils \
    && apt-get clean && apt-get autoremove && rm -rf /var/lib/apt/lists/*

USER torizon
