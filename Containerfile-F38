FROM registry.fedoraproject.org/fedora-minimal
USER 0
RUN microdnf install -y git ostree rpm-ostree skopeo selinux-policy-targeted podman skopeo

RUN mkdir -p /usr/share/distribution-gpg-keys/centos

COPY ./RPM-GPG-KEY-CentOS-Official /usr/share/distribution-gpg-keys/centos/RPM-GPG-KEY-CentOS-Official

WORKDIR /root
