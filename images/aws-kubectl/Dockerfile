FROM amazon/aws-cli:latest@sha256:733d5be1015825e4038c6016f3fa9954868ddee1f611b73be795a9cc2e706bfd AS aws
FROM bitnami/kubectl:latest@sha256:26837860fa038ce221416ee0fd211a0ee300f67e24e88faecca0423088400b99 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
