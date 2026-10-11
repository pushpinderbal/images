FROM amazon/aws-cli:latest@sha256:ce44b800602264c12298bbf3399055a4cefdb9ed4a098abe564afe26e7071bce AS aws
FROM bitnami/kubectl:latest@sha256:999d5eb28f404b45f15117f2a110ff23c6164f76edac261d75d783b6e88252b7 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
