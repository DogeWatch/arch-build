FROM archlinux:latest

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
RUN date

COPY entrypoint.sh /entrypoint.sh
COPY makepkg.conf.tmpl /usr/share/devtools/makepkg-x86_64.conf
RUN sudo chmod 777 /entrypoint.sh

USER root

ENTRYPOINT ["/entrypoint.sh"]