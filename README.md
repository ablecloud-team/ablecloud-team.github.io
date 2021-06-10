## ablecloud.io 홈페이지 리파지터리

ABLECLOUD 홈페이지 소스코드를 위한 리파지터리입니다.
홈페이지는 github.io를 통해 관리되며 Jekyll 블로그 앱 및 테마를 이용해 홈페이지 테마를 적용합니다.
따라서 개발환경을 구성하기 위해서는 소스코드 클론 뿐 아니라, Jekyll을 구성해야 합니다. 

### 개발환경 구성

다음과 같이 개발환경을 구성합니다. 

1. CentOS 8 서버 또는 가상머신을 준비합니다. 
2. Development Tools 패키지 그룹을 설치합니다. 
   ```
   $ dnf groupinstall "Development Tools"
   ```
3. Ruby 및 Ruby Devel을 설치합니다. 
   ```
   $ dnf install ruby ruby-devel
   ```
4. RubyGems를 이용해 bundler를 설치합니다.
   ```
   $ gem install bundler
   ```
   
### 리파지터리 클론

개발환경을 구성한 후 홈페이지 리파지터리의 소스를 Folk 한 후 Clone 합니다. 

> 소스코드 리파지터리를 개인이 개발할 때는 반드시 개인 계정으로 Folk 한 후 Folk한 소스를 사용합니다. 수정된 소스를 원본 소스에 반영하고자 하는 경우 Pull Request를 통해 Pull을 요청하고 관리자의 승인을 통해 소스코드가 반영되도록 해야 합니다.

소스 디렉토리로 이동해서 다음의 파일을 삭제합니다. 그 

### 개발 서버 실행

소스코드를 클론한 후 변경된 소스코드를 확인하기 위해서는 개발서버에 Jekyll 테마를 위한 번들을 설치해야 합니다. 번들 설치 및 개발 서버 실행은 모두 소스코드가 클론 된 디렉토리에서 해야 합니다. 

```
$ cd <repo_dir>
$ bundle install
```

필요한 번들을 설치한 후 테스트용 Jekyll 웹 서버를 구동합니다.


```
$ bundle exec jekyll serve -H <IP Addr> -P <port>
```

웹 브라우저를 이용해 접속하여 정상 여부를 확인합니다. 
