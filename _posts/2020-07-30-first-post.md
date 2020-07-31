---
title:  "Github Pages 작성"
excerpt: "yusunu.github.io"

categories:
  - Blog
tags:
  - Blog
last_modified_at: 2020-07-29T08:06:00-05:00
---



### Repository 생성(Github)
- Create a new repository

사용자명을 접두어로한 `{username}.github.io`형식의 레포지토리를 생성
<code>yusunu.github.io</code>

### Github page 초기파일 생성(Github)
- Create new files

index.html  
or  
index.MD  

### 확인 

<https://yusunu.github.io>

### Repository 관리(Local)
```sh
git clone https://github.com/yusunu/yusunu.github.io.git
```

### Jekyll 適用(Local)
#### install ruby + Jekyll 
```sh
sudo apt install ruby-full build-essential zlib1g-dev
#ユーザ単位
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
ruby -v
gem -v
gem install jekyll bundler
jekyll yusunu.github.io.git
jekyll -v
bundle install
bundle exec jekyll serve
```