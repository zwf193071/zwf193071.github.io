---
layout: post
title: create my blog
categories: jekyll
image: jekyll.jpg
date: 2019-1-14 15:47:05
pid: 20190114-154705
pin: 9
---
jekyll搭建博客时，遇到很多问题，印象比较深刻的是，更换博客主题风格的时候，运行jekyll serve命令时，会提示:
```
You have already activated public_suffix 3.0.3, but your Gemfile requires public_suffix 2.0.5
```
 以上一系列类似的版本问题，知道大概原因是_config.yml里面的文件版本与Gemfile要求的不一致，但总不能一行行傻傻地
修改。通过运行```bundle install```加上```bundle update```命令，再次运行```jekyll serve```命令时，发现仍然出现版本提示错误，改用
```bundle exec jekyll serve```命令时，本地可以成功运行，该命令确保你使用的便是Gemfile配置的gem版本

Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help