FROM amazon/aws-cli:latest@sha256:82905aa8fdab6e2403b40dceec12dc33aea2535a4c2a6f13d596d98501951105 AS aws
FROM bitnami/kubectl:latest@sha256:ab90e1058e5a658cc94b4e7eb6d48e5758cfd6d77b5dd1869513aec3a3054673 AS kube

FROM aws
COPY --from=kube /opt/bitnami/kubectl/bin/kubectl /usr/local/bin/kubectl
ENTRYPOINT []
CMD ["/bin/bash"]
