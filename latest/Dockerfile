FROM fedora:35

RUN dnf install -yq iputils net-tools iproute telnet bind-utils && \
    dnf install -y nftables nftables iptables iproute && \
    dnf install -y nc tcpdump nmap && \
    dnf clean all
RUN echo "alias ll='ls -al'" >> /etc/bashrc && \
    echo "alias ..='cd ..'" >> /etc/bashrc && \
    echo "alias ...='cd ../..'" >> /etc/bashrc && \
    echo "alias tailf='tail -f'" >> /etc/bashrc
