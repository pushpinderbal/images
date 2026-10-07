FROM amazon/aws-cli:latest@sha256:3dacc5db57c923c4223e949795f538ecf1f2212b2b7d5a028b47b97f91564c0d AS aws
FROM bitnami/kubectl:latest@sha256:f7f9e4f64d9e114650c115a4ac6fd383394b3d494061a8f17b1a0f6c8d55bc25 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
