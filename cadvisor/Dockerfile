FROM google/cadvisor:v0.27.4
LABEL maintainer "Rodrigo Araujo Cavalcante <rodrigoibka@gmail.com>"

ADD auth.htpasswd /

EXPOSE 8000
ENTRYPOINT ["/usr/bin/cadvisor", "--http_auth_file", "auth.htpasswd", "--http_auth_realm", "localhost"]
