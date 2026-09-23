FROM amazon/aws-cli:latest@sha256:337494c2047176fe9abcf45a5d1eaf1c2c62cae40953284fb1143b5c6170f065 AS aws
FROM bitnami/kubectl:latest@sha256:6e9c5284a0dac06e84de9f4d97852d2e6513442ee7ec3a66d35009eec86e1e62 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
