---
layout: post
title:  "Write Blog Using Jekyll and GitHub.io!"
date:   2018-08-17 10:10:52 +0800
categories: coding exp
---

# Win10使用jekyll写个人博客并托管到GitHub.io

## 缘起
> 想要搭建自己的个人技术博客，基于GitHub的[GitHub Pages][GitHub Pages]当然是最好的选择。

## 环境

| OS 名称   | Microsoft Windows 10 专业版 |
| 系统类型   | x64-based PC |


## 步骤
上Jekyll官方网站查阅[Windows使用指南][jekyllrb-windows]



1. [下载安装Ruby环境][ruby-install]
    
    Ruby+Devkit 2.5.1-2 (x64)
    
    PS: 检查ruby25/bin是否加入了[环境变量][path-env]
2. 修改包安装源（不能翻墙的话）

    $gem sources --remove https://rubygems.org/
    
    $gem sources -a https://gems.ruby-china.com/
3. 安装Jekyll环境
    
    $gem install jekyll bundler
4. 使用jekyll创建新项目

    $jekyll new myblog
    
    PS: 初次使用时这里Running bundle install 会卡住很久，我会手动退出，然后进入myblog目录执行$bundle install，会根据Gemfile文件去安装依赖。依赖安装完成后再使用new就很快了。
5. 运行网页服务器
    $cd myblog
    $jekyll serve



### 参考资料
[jekyll使用手册][jekyll-user-page]

[GitHub Pages]: https://pages.github.com/
[jekyllrb-windows]: https://jekyllrb.com/docs/windows/
[ruby-install]: https://rubyinstaller.org/downloads/
[path-env]: https://baike.baidu.com/item/%E7%8E%AF%E5%A2%83%E5%8F%98%E9%87%8F/1730949
[jekyll-user-page]: http://www.lijiaocn.com/%E6%8A%80%E5%B7%A7/2017/05/15/jekyll.html