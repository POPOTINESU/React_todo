# ベースイメージの指定
FROM node:21.7-alpine
# 作業ディレクトリの設定
WORKDIR /usr/src/app
# package.json と package-lock.json (もし存在する場合) をコピー
COPY package.json yarn.lock ./
# 依存関係のインストール
RUN yarn install
# アプリケーションのソースをコピー
COPY . .