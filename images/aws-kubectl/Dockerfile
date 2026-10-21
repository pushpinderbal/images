FROM amazon/aws-cli:latest@sha256:efe32e825cf203652eaca3e7e94679580274e7d567c39270aaa36a5144737108 AS aws
FROM bitnami/kubectl:latest@sha256:9b58231669c7c371ecd976626a61d72ae7e46326f30932e8934a087f5f26fbd8 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
