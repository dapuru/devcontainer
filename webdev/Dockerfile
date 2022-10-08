# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.245.2/containers/debian/.devcontainer/base.Dockerfile

# [Choice] Debian version (use bullseye on local arm64/Apple Silicon): bullseye, buster
ARG VARIANT="buster"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-${VARIANT}

# ** [Optional] Uncomment this section to install additional packages. **
 RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
     && apt-get -y install --no-install-recommends mariadb-server mariadb-client lighttpd php php-cli php-common php-fpm php-mysql


# TODO
# https://www.rosehosting.com/blog/how-to-install-lighttpd-on-debian-9/

# /etc/php/7.0/fpm/php.ini
# Change cgi.fix_pathinfo value to 1

# /etc/php/7.0/fpm/pool.d/www.conf
# find line listen = /run/php/php7.0-fpm.sock
# replace with listen = 127.0.0.1:9000

