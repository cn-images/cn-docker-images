# syntax=docker/dockerfile:1
FROM archlinux:base

COPY <<"EOF" /etc/pacman.d/mirrorlist
Server = https://mirrors.ustc.edu.cn/archlinux/$repo/os/$arch
Server = https://mirrors.tuna.tsinghua.edu.cn/archlinux/$repo/os/$arch
Server = https://mirror.sjtu.edu.cn/archlinux/$repo/os/$arch
EOF

CMD ["/usr/bin/bash"]
