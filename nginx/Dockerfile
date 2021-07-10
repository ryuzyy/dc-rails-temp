FROM nginx:1.15.8

RUN rm -f /etc/nginx/conf.d/*

#confファイルを移し替える
ADD nginx.conf /etc/nginx/conf.d/dc-rails-temp.conf

#デーモンオフ(フォアグラウンドで動かすように設定)
CMD /usr/sbin/nginx -g 'deamon off;' -c /etc/nginx/nginx.conf
