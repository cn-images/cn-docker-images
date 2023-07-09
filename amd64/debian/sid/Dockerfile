FROM --platform=linux/amd64 debian:sid
RUN sed -i -r \
	's#^URIs:.*$#URIs: http://mirrors.ustc.edu.cn/debian#' \
	/etc/apt/sources.list.d/debian.sources
CMD ["bash"]
