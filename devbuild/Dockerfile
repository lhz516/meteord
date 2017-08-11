FROM hanzluo/meteord:base
MAINTAINER Hanz Luo

ARG NODE_VERSION
ENV NODE_VERSION ${NODE_VERSION:-8.3.0}

ONBUILD RUN bash $METEORD_DIR/lib/install_meteor.sh
ONBUILD COPY ./ /app
ONBUILD RUN bash $METEORD_DIR/lib/build_app.sh