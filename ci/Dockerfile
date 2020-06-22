FROM nginx
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get -o DPkg::Options::="--force-confnew" install -y cowsay
COPY say /data/say
RUN echo "<html><body><pre>$(/usr/games/cowsay < /data/say)</pre></body></html>" > /usr/share/nginx/html/index.html
