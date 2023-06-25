# 使うDockerイメージ
FROM mysql

# ポートを開ける
# mysqlのデフォルトポート
EXPOSE 3306

# MySQL設定ファイルをイメージ内にコピー
COPY my.cnf /etc/mysql/conf.d/my.cnf

# docker run時に実行される
CMD ["mysqld"]
