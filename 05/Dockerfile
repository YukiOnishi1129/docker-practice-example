# このDockerfikeから「smaple」というイメージを作成するコマンド
# docker build -t sample:1.0 05

# ベースイメージの設定
# FROM centos:centos7

# STEP1: Ubuntu
FROM ubuntu:latest

# STEP2: Nginx
RUN apt-get update && apt-get install -y -q nginx

# STEP3: ファイルコピー
COPY index.html /usr/share/nginx/html/

# STEP4: Nginxの起動
CMD ["nginx", "-g", "daemon off;"]
