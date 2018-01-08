Renew certificate crontab

    29 2 * * 1 echo $(date -u) >> /var/log/le-renew.log
    30 2 * * 1 /usr/bin/certbot renew >> /var/log/le-renew.log
    35 2 * * 1 /usr/sbin/service nginx reload

Create certificate

    certbot certonly --nginx -d rusiczki.net -d www.rusiczki.net -d content.rusiczki.net
