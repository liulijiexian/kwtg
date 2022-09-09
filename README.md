总体格式按照这样写就可以了，具体细节我也不太清楚了，因为网上这方面的教程比较少，所以是东找西找的（要是有中文官方文档就好了），反正就是api文件底下index.py（flask的app.py修改为index.py），然后根据你的根目录导入对应本地文件。其次写路由时要后面加 `/`，如：/getMusicMain/、/getMusicUrl/ 。因为 vercel 里 /getMusicMain 和 /getMusicMain/ 不是一个意思，/getMusicMain 代表目录。同时 vercel.json 里也要添加一条： "trailingSlash": true 。这条会让 /getMusicUrl/ 显示出来，而不是输入 /getMusicUrl/ 显示 /getMusicUrl

