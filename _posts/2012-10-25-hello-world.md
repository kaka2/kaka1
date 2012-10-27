---
layout: page 
title: Hello World 
tagline: 
---
{% include JB/setup %}

## 軟硬環境和配置：

>PC：Win XP  
Git for win: [msysgit](http://msysgit.github.com/)  
Ruby和devkit: [rubyinstaller](http://rubyinstaller.org/downloads/)  
RubyGems: [rubygems](http://rubygems.org/pages/download)  
Jekyll: [Jekyll](http://jekyllbootstrap.com/usage/jekyll-quick-start.html)  
Jekyll-Bootstrap: [Jekyll Bootstrap](http://jekyllbootstrap.com)  


## 知識點  

1. 利用github pages自動創建gh-pages:    
推薦非常棒的: [Github Pages極簡教程](http://yanping.me/cn/blog/2012/03/18/github-pages-step-by-step/)

2.由於步驟1建立的gh-pages中，含有非步驟2中的文件，所以:    
[如何刪除 remote 的文件?](http://hi.baidu.com/zairl23/item/4a34c60084108fd01ef0464d)   
本地(gh-pages)操作命令：   

>git status   
git rm <files>    
git commit -a -m "delete"    
git push origin gh-pages   

3.clone該gh-pages所在的repo到本地 ,保留.git目錄  

>git clone git@github.com:username/repo.git  

4.將jekyll-bootstrap的源碼clone到本地  
刪掉此處的.git目錄 ,剩下的文件複製到步驟2的repo目錄下, 配置_config.yml等    

然後上傳  
>git add .  
git commit -a -m "delete"   
git push origin ph-pages   

5.其他命令    
由項目主頁的project到gh-pages  
cd repo  
git branch gh-pages_name  
git checkout gh-pages_name   
