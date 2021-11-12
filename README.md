# Jekyll 테마

[About GitHub Pages and Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll)

----

## Homebrew
https://github.com/homebrew/install

### `brew` 제거
```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/uninstall.sh)"
```

### `brew` 설치
```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
##### *~/.bashrc* 수정
``` sh
# homebrew
eval "$(/opt/homebrew/bin/brew shellenv)"
```

----

## Jekyll

### `ruby` 설치
`ruby`를 설치하면 `gem`도 함께 설치됨
```sh
brew install ruby
```

###### *~/.bashrc* 수정
``` sh
# homebrew ruby
PATH="/opt/homebrew/opt/ruby/bin:$PATH"
PATH=$(gem environment gemdir)/bin:$PATH
```

### `jekyll` 설치
```sh
gem install jekyll
```

----

### 프로젝트 생성
```sh
mkdir PROJECT
cd PROJECT
jekyll new .
```

###### `webrick` 추가
```sh
bundle add webrick
```

[jekyll 사용법](https://jekyllrb.com/docs/usage/)
###### *./_site*에 빌드하기
```sh
jekyll build
```

###### 확인하기
```sh
jekyll serve
```
http://127.0.0.1:4000

----

## 테마 설정

###### https://github.com/topics/jekyll-theme

```sh
bundle add THEME-GEM-NAME
```