FROM amazon/aws-cli:latest@sha256:c8156a0e74e13929a42d7e60f0d4e14e7d28d980cd21822505d4bff80e5460c1 AS aws
FROM bitnami/kubectl:latest@sha256:6d9e8ad566a6d2dcb4a7a6120d030bd65bddbcc952246f4b31022834d9be7e02 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
