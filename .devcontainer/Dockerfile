FROM sel4_dev

RUN apt-get update && \
    apt-get install -y --no-install-recommends zsh && \
    apt-get clean autoclean && \
    apt-get autoremove --purge --yes && \
    rm -rf /var/lib/apt/lists/*

RUN useradd -u 501 -ms /bin/zsh nick
RUN adduser nick sudo
RUN echo 'nick ALL=(ALL) NOPASSWD:ALL' >>/etc/sudoers
