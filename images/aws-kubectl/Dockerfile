FROM amazon/aws-cli:latest@sha256:92de75724b6a746951f0e8b915d86bbccd7cb55aff96cd0cb4f7017272160780 AS aws
FROM bitnami/kubectl:latest@sha256:f7f9e4f64d9e114650c115a4ac6fd383394b3d494061a8f17b1a0f6c8d55bc25 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
