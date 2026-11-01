FROM amazon/aws-cli:latest@sha256:d557b3524475d70dd3104cf44d96568ee3188897b73a6ece2b37aa50e1af362f AS aws
FROM bitnami/kubectl:latest@sha256:bedd34c910e2a5ce9836813d16444af449d7fe07a29136d59f34e861e8e660c5 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
