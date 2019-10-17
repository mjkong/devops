# DevOps 실습

> String Boot 기반의 심플한 Web application을 Jenkins pipeline을 이용하여 Kubernetes에 디플로이
> 실습환경은 IBM Cloud의 Kubernetes Cluster 를 사용합니다.
> Jenkins는 Kubernetes 환경에 사전 설치되어 있는 형태로 Pipeline 작성 위주로 실습합니다.

## Github 프로젝트 가져오기
실습을 위해서 대상 애플리케이션을 각 개인 계정의 github로 fork 합니다. 
실습 대상 애플리케이션은 Spring Boot sample 중 하나 입니다.

다음의 링크로 접속하여 아래 화면과 같이 `fork`를 합니다.

https://github.com/spring-guides/gs-serving-web-content

![git fork](./images/git_fork.png)
![git fork](./images/git_fork2.png)

`fork`가 완료되었으면 `github`링크 주소를 저장해 둡니다. 향후 `Jenkins` 설정 시 사용하게 됩니다.

## Jenkins 계정 만들기 
실습을 위해서 Jenkins에 접속하여 각자 계정을 생성합니다. 각 자 `admin` 계정으로 로그인 한 뒤 `Left panel --> Manage Jenkins --> Manage Users 클릭 --> Left panel의 Create user 클릭` 

Jenkins link: http://173.193.112.66:30100

> 참고로 어드민 계정 정보는 다음과 같습니다.   

~~~
ID : admin
PW : passw0rd
~~~

![](./images/create_user.png)