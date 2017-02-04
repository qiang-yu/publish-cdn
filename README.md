# 这个工程是用于保存一些生成的发布文件


gfwlist
---

用于保存生成好的 gfwlist.conf 和  gfwlist_localdns.conf 文件，每天更新，如果你的DNS解析配置的是别的端口，可以按照下面的方式生成

   ```bash
   ## 把 8.8.8.8#53 替换成你需要的 dns 解析地址
   /bin/cat gfwlist.conf | /bin/sed "s/8.8.8.8#53/127.0.0.1#7070/g" > /tmp/gfwlist_localdns.conf
   ```

