FROM amazon/aws-cli:latest@sha256:eccdb3ec77e159d43ca6a750a70738c546883138be7f094498294a1477ec7e42 AS aws
FROM bitnami/kubectl:latest@sha256:8f59408f9e896fc8992a0660a56687545bd06751f26531b4a26fca6d5dc7562d AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
