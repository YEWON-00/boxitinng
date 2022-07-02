> **GitHub에 코드를 올리는 과정 복습**
> 
1. 내 컴퓨터 프로젝트 폴더에 '여기에서 Git을 쓸거다!' 라고 명령 ⇒ git init
2. 코딩
3. 내가 변경한 파일 중 올리길 원하는 것만 선택
4. 선택한 파일들을 한 덩어리로 만들고 설명 적기
5. **GitHub 사이트에서 프로젝트 저장소 만들기**
6. **내 컴퓨터 프로젝트 폴더에 GitHub 저장소 주소 알려주기 ⇒ git remote add**
7. **내 컴퓨터에 만들었던 덩어리 GitHub에 올리기 ⇒ git push**

> **로컬 저장소와 원격 저장소**
> 

우리가 앞서 실습 했던 것들은 '로컬 저장소'에서 저장되고 있던 것!

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/beacbeb5-0551-4cac-95c9-a3169c64e6d1/.jpg](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/beacbeb5-0551-4cac-95c9-a3169c64e6d1/.jpg)

**로컬 저장소에 있는 버전을 원격 저장소에 올리는 명령어 'push'**

> **원격 저장소 GitHub에서 만들고 커밋 푸시하기**
> 
1. GitHub에 로그인해서 Boxiting 저장소 생성
2. 내 컴퓨터 boxiting-cat 폴더에 GitHub 저장소 주소 알려주기

```bash
git remote add origin https://github/아이디/이름.git
```

- remote add ⇒ 원격 저장소를 추가하는 명령어
- origin ⇒ 원격 저장소를 origin 이라는 이름으로 추가한다는 말

 3. 만든 커밋 푸시하기

```bash
git push origin master
```

- master ⇒ '브랜치'라는 개념. 기본 브랜치의 이름이 master
- [브랜치란?](https://git-scm.com/book/ko/v2/Git-%EB%B8%8C%EB%9E%9C%EC%B9%98-%EB%B8%8C%EB%9E%9C%EC%B9%98%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80)

4. GitHub 사이트에서 올라간 커밋 확인

> GitHub
> 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/753660bc-3ca1-43b9-b424-e0963f2f28d3/.jpg](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/753660bc-3ca1-43b9-b424-e0963f2f28d3/.jpg)

> README 란?
> 
1. New repository - 새로운 저장소 만들기
2. Import repository - 저장소 가져오기
3. New gist - 코드 조각을 올리고 싶을 때
4. New organization - 팀플시 팀 이름으로 생성 가능
5. New project

새 repository를 만들 때 보이는 창으로 이 저장소를 만들 때 [README.md](http://readme.md) 파일도 같이 만들겠냐고 묻는 옵션

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a8dc495a-24ba-460e-b13e-7592a0fda57c/.jpg](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a8dc495a-24ba-460e-b13e-7592a0fda57c/.jpg)

**README.md의 역할** ⇒ *github 저장소에 처음 들어왔을때 이 소스코드가 무엇을 하는지, 저장소에 온 사람들이 어떤 정보를 읽었으면 좋겠는지 명시하는 역할*

ex) 오픈소스 설치 방법, 오픈소스 지원 범위, 오픈소스의 documetation, 라이센스

- gitignore 옵션: 만약 node를 선택 시 .gitignore라는 파일을 생성해주는데 여러가지 텍스트가 작성되어 있음. 그 텍스트에는 노드 모듈스 등등이 있는데 이렇게 .gitignore에 텍스트를 추가하면 우리가 git에 add를 해서 파일에 commit을 추가 시 거기에서 무시가 됨. 예를 들어 이 폴더는 내 로컬에서만 쓰고싶어, 비밀 키가 있어서 노출되면 안돼 하면 .gitignore에 그 폴더를 추가하면 됨. node 프로젝트 시 외부 라이브러리를 많이 사용할텐데 외부 라이브러리를 굳이 github에 올릴 필요가 없으니까 git ignore에 node modules라는 폴더를 추가하면 됨.

> 실습 화면
> 

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f016ae1f-72df-4371-9265-fb5748adab77/.jpg](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f016ae1f-72df-4371-9265-fb5748adab77/.jpg)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/64dfc0c0-f7ca-4b66-af31-fc1629cfc4f2/sdf.jpg](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/64dfc0c0-f7ca-4b66-af31-fc1629cfc4f2/sdf.jpg)