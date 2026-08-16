ARG HUGO_VERSION=latest
FROM ghcr.io/gohugoio/hugo:${HUGO_VERSION}

# User metadata
ARG USERNAME=hugo

# Create the user
USER root
RUN apk add --no-cache make shadow && \
    chsh $USERNAME --shell /bin/ash

USER $USERNAME
