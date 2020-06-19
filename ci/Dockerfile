FROM nginx
RUN apt-get update && apt-get install -y cowsay
COPY say /data/say
RUN echo "<html><body><pre>$(/usr/games/cowsay < /data/say)</pre></body></html>" > /usr/share/nginx/html/index.html
