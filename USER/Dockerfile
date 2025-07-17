FROM almalinux:9
RUN dnf install nginx -y
RUN useradd monnish
USER monnish
CMD ["nginx","-g","daemon off;"]
