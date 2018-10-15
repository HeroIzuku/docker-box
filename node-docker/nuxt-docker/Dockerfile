FROM centos
ENV name node-docker
ENV NODE_ENV=production
ENV HOST 0.0.0.0
WORKDIR /root/source/node
COPY node-v10.12.0-linux-x64.tar.xz /root/source/node/node-v10.12.0-linux-x64.tar.xz
RUN  tar xvf node-v10.12.0-linux-x64.tar.xz && \ 
     ln -s /root/source/node/node-v10.12.0-linux-x64/bin/node /usr/local/bin/node && \
     ln -s /root/source/node/node-v10.12.0-linux-x64/bin/npm /usr/local/bin/npm && \
     ln -s /root/source/node/node-v10.12.0-linux-x64/bin/npx /usr/local/bin/npx
WORKDIR /apps
EXPOSE 3000
# 映射开发目录  -v host/path:container/path
# 映射本地端口  -p 8081:80
