FROM mcr.microsoft.com/devcontainers/dotnet:1-10.0-noble

# The base devcontainer image ships with a stale Yarn APT source. Its repository is missing
# the required GPG key, so feature installs fail during `apt-get update` with
# `NO_PUBKEY 62D54FD4003F6525`.
RUN rm -f /etc/apt/sources.list.d/yarn.list \
    /etc/apt/sources.list.d/yarn.sources \
    /etc/apt/keyrings/yarn.gpg \
    /usr/share/keyrings/yarn.gpg
