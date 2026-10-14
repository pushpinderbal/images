FROM amazon/aws-cli:latest@sha256:ed3233c28ad56d6a66e9e7623a495ab2d7eb08d425f8eea0fdbdfacb12de2ba8 AS aws
FROM bitnami/kubectl:latest@sha256:dbe04f493d362c47db291edb3382aeb56cf430a6271daa56311f5b8e82fecf2a AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
