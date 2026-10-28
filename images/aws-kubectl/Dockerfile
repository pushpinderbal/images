FROM amazon/aws-cli:latest@sha256:6014c77975a4ae237395924cc821333f20bf87c91964a45dd4ed5f3b13b424f5 AS aws
FROM bitnami/kubectl:latest@sha256:eaf442416e6f6b37ea76cc03dbdacc1d85f4c061670df7974dd1387288a11e50 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
