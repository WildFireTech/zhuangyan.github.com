---
layout: post
title: 这是个测试页面
tags: ["nodejs","服务器"]
---
  ǰ��ͬѧд��һ��nodejs����վ�����Ұ�æ���������ǵ�web�������ϡ�����ǰ����û�������������ϲ����nodejs�ķ�����̨������������Ҳֻ��һ��nginx+uwsgi����վ�����С�
����nginx���Ǻܼ򵥵ģ�ֱ����nginx.conf�����һ��server���þͿ����ˡ�

{% highlight nginx %}
server { listen 80; server_name mui.zhugyan.cn; location / { proxy_pass http://localhost:3000; } }
{% endhighlight }

Ȼ������nohup�����Ժ�̨��ʽ����nodejs��web����

{% highlight bash %}
nohup node /root/bsml/bin/www &
{% endhighlight }

����nodejs����Ϳ���ͨ�������������ˡ�
