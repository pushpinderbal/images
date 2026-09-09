FROM amazon/aws-cli:latest@sha256:be7c8de0160a2e2269159bc2634c002c85b1a21d6322e2ad513b3f7f48325c99 AS aws
FROM bitnami/kubectl:latest@sha256:b29d8c1665b70817259ceecaea16ab27aab6368b48daf485d19436c809067492 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
