FROM centos
ENV name node-docker
WORKDIR /apps/node
COPY node-v10.12.0-linux-x64.tar.xz /apps/node/node-v10.12.0-linux-x64.tar.xz
RUN  tar xvf node-v10.12.0-linux-x64.tar.xz && \ 
     ln -s /apps/node/node-v10.12.0-linux-x64/bin/node /usr/local/bin/node && \
     ln -s /apps/node/node-v10.12.0-linux-x64/bin/npm /usr/local/bin/npm
# 映射开发目录  -v path:path