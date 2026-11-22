FROM amazon/aws-cli:latest@sha256:b0102d2269f87d8531d931c1a59e248101ace586886e6c077058d94c1c37b846 AS aws
FROM bitnami/kubectl:latest@sha256:8919c149c2e3d6860e0143c117900e64d71395172aaef0e01e604bb98c8e7ce0 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
