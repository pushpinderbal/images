FROM amazon/aws-cli:latest@sha256:fdd8d1fcbea9c371678dee5a40df8b178c7a781b4586605756ee28114c97ead6 AS aws
FROM bitnami/kubectl:latest@sha256:ab90e1058e5a658cc94b4e7eb6d48e5758cfd6d77b5dd1869513aec3a3054673 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
