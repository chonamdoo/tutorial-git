# Tutorial GIT
w

### 어떻게 깃을 사용하는지 빠르게 알아봅시다.
> Quick learn How to use the Git.

### 시작하며

##### 깃을 왜 사용하죠?

- 빠른 협업환경 조성
- 누가 언제 무엇을 왜 수정했는지 코드리뷰가 가능
- IssueTracker 및 Migrate 지원
- GitHub를 이용하여 자신의 git을 쉽게 전파, 공유가 가능
- Continuous Integration (지속적인 통합) 지원
- VisualStudio, Eclipse, Android Studio 등 많은 부분에서 Git연동 제공

- **결국 대게는 협업을 위해서 사용**

##### 깃이 어떤 역할을 하는건가요?

- 소스 병합
- 소스 리비전 관리
- 소스 배포
- 소스 태깅
- 소스 기록, 업로드
- 소스 변경사항 검토

##### 깃은 어디에서 지원하나요?

- Windows
- Mac
- Linux, Unix 계열

----

### 깃의 기능

#### 깃의 설정 (클라이언트)

- 깃은 초기에 `git init` 작업을 진행합니다
- 혹여나 GitHub에서 클론을 받은경우 이 작업은 필요하지 않습니다.
- 아래 샘플 코드를 확인해주세요.

 ```shell
    git init
```
- `git init`을 하셨으면 Git 리모트를 설정하실 수 있습니다.
- Git 리모트란 Git을 원격저장소에 저장하는 앤드포인트를 의미합니다.

 ```shell
   git remote add origin https://github.com/KennethanCeyer/tutorial.git
```
#### 소스 기록, 업로드

- 소스를 업로드 하기 위해서는 `git add` 명령어를 이용합니다.
- 샘플을 참고하세요

 ```shell
    git add *
```

- ignore 파일이나, 삭제한 파일 이력까지 커밋을 하실 경우, `-f` 옵션을 이용합니다.

 ```shell
    git add * -f
```

#### 소스 커밋, 메시지 작성

- 소스를 커밋하시면 `Tracked` 상태에서 `Strage` 상태로 변경됩니다.
- 파일 추적상태의 경우 `git status` 명령을 이용해서 확인합니다.

 ```shell
    git status
 ```
