## 安装依赖：npm install --force 如果安装出错，可以先 rm -rf package-lock.json 后重试
- .env 文件放在根目录
- generate NEXTAUTH_SECRET: openssl rand -base64 32 复制到.env 的 NEXTAUTH_SECRET
- 初始化数据库 prisma 和连接 postgresql（没有修改 prisma schema 和 postgresql 的地址的，不需要执行） npx prisma migrate dev
- 启动程序： npm run dev
