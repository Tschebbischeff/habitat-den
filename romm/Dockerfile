FROM rommapp/romm:latest

RUN apk upgrade --no-cache -a; \
    apk add --no-cache patch

COPY ./patches /habitat-patches
RUN patch "/backend/handler/auth/base_handler.py" <"/habitat-patches/base_handler.py.patch"
RUN rm -rf /habitat-patches