# syntax=docker/dockerfile:1
FROM debian:sid

RUN <<-EOF
	if [ "$(uname --machine)" = 'riscv64' ]; then
		sed -i -r \
			's#^URIs:.*$#URIs: http://mirrors.aliyun.com/debian-ports#' \
			/etc/apt/sources.list.d/debian.sources
	else
		sed -i -r \
			's#^URIs:.*$#URIs: http://mirrors.ustc.edu.cn/debian#' \
			/etc/apt/sources.list.d/debian.sources
	fi
EOF

CMD ["bash"]
