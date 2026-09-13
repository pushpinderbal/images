FROM amazon/aws-cli:latest@sha256:e8467f2c319f9bc9a1471808a69949a76915e9c95eaf4a09ece9f9e85fd32747 AS aws
FROM bitnami/kubectl:latest@sha256:b29d8c1665b70817259ceecaea16ab27aab6368b48daf485d19436c809067492 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
