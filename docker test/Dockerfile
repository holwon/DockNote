# FROM 必须是第一个, 指定 baseImage
# 这里使用 alpine 版的 node, alpine是一个很小的linux
FROM node:19-alpine3.16
# 这里复制所有的应用程序文件到 Image 的 app 目录下, app目录会自动创建
COPY . app

# CMD 是希望执行的命令, 由于创建了 app 目录所以需要加一个/app
# Dockerfile中只能有一条CMD指令。
# 注: 不要加中括号, 命令和文件名需要分开

# CMD "node" "/app/app.js" 

# 或者说指定工作目录, 在设置了工作区之后的所有命令都假的在工作区目录
WORKDIR /app
# CMD [ "node app.js" ]
CMD "node" "app.js"