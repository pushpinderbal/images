FROM amazon/aws-cli:latest@sha256:0da258e32b17cc468b2e8812c8d93f5732561b901357c43a207baae0567b195a AS aws
FROM bitnami/kubectl:latest@sha256:8f59408f9e896fc8992a0660a56687545bd06751f26531b4a26fca6d5dc7562d AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
