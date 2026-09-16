FROM amazon/aws-cli:latest@sha256:eedfdcb56e9a1b02fabcf656977ca226f40860c6672aca41d435e036bc95a075 AS aws
FROM bitnami/kubectl:latest@sha256:b29d8c1665b70817259ceecaea16ab27aab6368b48daf485d19436c809067492 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
