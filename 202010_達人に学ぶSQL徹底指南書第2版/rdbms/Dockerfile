FROM postgres:10.1

# ロケール設定
RUN localedef -i ja_JP -c -f UTF-8 -A /usr/share/locale/locale.alias ja_JP.UTF-8
ENV LANG ja_JP.utf8

# 作成した設定ファイルを/etc/postgresql以下にコピー
COPY ./conf/my-postgresql-10.1.conf /etc/postgresql/postgresql.conf

CMD ["-c", "config_file=/etc/postgresql/postgresql.conf"]