FROM gcc

RUN git clone https://github.com/ecsv/gliden64-cache-extract.git /tmp/gce && \
    cd /tmp/gce && \
    make && \
    mv gliden64_cache_extract /bin && \
    chmod +x /bin/gliden64_cache_extract && \
    rm -rf /tmp/gce

COPY entrypoint /bin
ENTRYPOINT [ "run" ]

VOLUME /textures
WORKDIR /workdir