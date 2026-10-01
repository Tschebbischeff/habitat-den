ARG ROMM_VERSION
FROM rommapp/romm:${ROMM_VERSION}

RUN apk upgrade --no-cache -a; \
    apk add --no-cache patch

COPY ./patches /habitat-patches
RUN patch -f -r - "/backend/handler/auth/base_handler.py" <"/habitat-patches/base_handler.py.patch"
RUN rm -rf /habitat-patches