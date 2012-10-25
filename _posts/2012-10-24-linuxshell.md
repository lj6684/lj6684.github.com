---
layout: post
title: "Linux下Shell设置"
description: "Linux环境下Shell的设置和切换"
category: tech
tags: [Linux, Shell, zsh]
---
{% include JB/setup %}

### Linux下推荐安装zsh
[zsh](https://github.com/robbyrussell/oh-my-zsh/) 功能比系统自带的bash强大很多，而且集成有好多开发用插件，推荐安装使用
{% highlight bash %}
sudo apt-get install curl
sudo apt-get install zsh
sudo apt-get install git
curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh
{% endhighlight %}			

### 将默认的Shell设置为zsh
{% highlight bash %}
chsh -s /bin/zsh
{% endhighlight %}
需要用户重新登陆后生效

###同理还原bash的命令是
{% highlight bash %}
chsh -s /bin/bash
{% endhighlight %}

### Linux下查看本机安装有哪些Shell
{% highlight bash %}
cat /etc/shells
{% endhighlight %}

### 查看本机使用的默认Shell
{% highlight bash %}
echo $SHELL
{% endhighlight %}