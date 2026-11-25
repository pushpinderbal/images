FROM amazon/aws-cli:latest@sha256:271de464e935f765aa2afb6ec69881e9f4a9afd3e978214a2b5f5ddcbbc161b5 AS aws
FROM bitnami/kubectl:latest@sha256:ae71f848f057a71029d092e98548cabf7cd17b11da0adad0a8f4145a9c87c830 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
