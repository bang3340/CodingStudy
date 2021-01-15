## 0. Review

Git을 이용한 프로젝트 작업 흐름

## 정리
정리 영상 : https://www.youtube.com/watch?v=YFNQwo7iTNc (노마드 코더)

### Git(깃)?

1. 버전관리 프로그램
2. 기록을 통째로 저장 하는 것이 아닌 달라진 부분만 기록 함 (효율적인 방법)
3. Branch를 이용하여 개발 코드 관리가 용이함

### GitHub(깃헙)?

1. git 데이터를 온라인에 저장해주는 사이트
2. 코드 공유가 가능하며 온라인으로 공동개발이 가능하다
3. 오픈소스들이 매우 많다 
4. ‘개발자들의 놀이터’, ‘프로그래머’들의 페이스북이다 

---------------------------------------------------------------------
GitHub(가입 & 설치하기)
링크 : https://post.naver.com/viewer/postView.nhn?volumeNo=24622891

깃헙 작업 흐름:
:https://velog.io/@dev_taehyun/Git%EC%9D%98-%EC%9E%91%EC%97%85-%ED%9D%90%EB%A6%84%EC%9D%84-%EC%95%8C%EA%B3%A0-%ED%9A%A8%EC%9C%A8%EC%A0%81%EC%9C%BC%EB%A1%9C-%EA%B4%80%EB%A6%AC%ED%95%98%EC%9E%90

## 1. Git & GitHub
GitHub(가입 & 설치하기)

0. Git(깃)에서 쓰는 주요 용어 정리 
영상 링크 : https://www.youtube.com/watch?v=PiQAwOxl52E (코드종)

- Working Directory = ‘내가 작업하는 공간(도화지)’
- Snapshot = ‘내가 작업하는 공간을 그대로 찍어둔 것’
- Repository = ‘사진이 저장되는 사진첩’ = Git repository
- Commit = ‘스냅샷을 사진첩에 넣는 행위’
- Checkout = ‘repository에 있는 특정 커밋 내용을 현재 W-D로 가져오는 행위’
- Branch = ‘ 나뭇가지와 같이 나눠진 갈래’


### 해시(hash)란?
다양한 길이를 가진 데이터를 고정된 길이를 가진 데이터로 매핑(mapping)한 값이다. 해시는 암호학에 있어서 매우 중요한 요소이며, 블록체인(blockchain)을 구현하기 위한 핵심 기술이다.


정리 영상 : https://www.youtube.com/watch?v=Bd35Ze7-dIw (얄팍한 코딩사전)

1. GitHub DeskTop
링크 : https://post.naver.com/viewer/postView.nhn?volumeNo=24622891

#### * 원격저장소(Repository)란?
원격으로 외부에 접속해 사용하는 저장소이다.
즉, 로컬에서 작업한 Git 프로젝트 저장소가 있는 로컬이 아닌 외부의 원격저장소이다.

#### * Github Desktop?
github를 CLI(Command-Line user Interface)방식이 아닌
GUI(그래픽 유저 인터페이스)방식으로 쉽게 사용할 수 있게 만든 프로그램입니다.

#### * 커밋(commit)?
이 파일의 수정이 끝났다는 의미로 로컬저장소에 저장하는 것

#### * 푸시(push)?
로컬 Staged에 저장된 파일을 원격 저장소(깃허브 사이트)에 저장하는 것입니다.


## 2. 깃 사용방법 


3. 마크다운(Markdown)을 이용한 Readme.md 파일 작성하기

영상 링크: https://www.youtube.com/watch?v=dUbp9wAy178 

마크다운(markdown)?
일반 텍스트 기반의 마크업언어로 README.md 파일이나 온라인 문서, 혹은 일반 텍스트 편집기로 문서 양식을 편집할 때 쉽게 쓰고 읽을 수 있으며 HTML로 변환이 가능하다.

* 마크업 언어란?
마크업 언어(markup 言語, markup language)는 태그 등을 이용하여 문서나 데이터의 구조를 명기하는 언어의 한 가지이다.
태그는 원래 텍스트와는 별도로 원고의 교정부호와 주석을 표현하기 위한 것이었으나 용도가 점차 확장되어 문서의 구조를 표현하는 역할을 하게 되었다. 이러한 태그 방법의 체계를 마크업 언어라 한다. 일반적으로 데이터를 기술하는 정도로만 사용되기에 프로그래밍 언어와는 구별된다.

굳이 어렵게 생각할 필요 없이, 책에 볼펜으로 밑줄을 긋는 행위도 그 내용이 중요하다는 의미를 나타내므로 마크업의 일종이라고 할 수 있다. 또는 그래픽 디자이너들한테 '책 표지는 배경을 무지개 그라데이션으로 넣어주시고 제목은 중앙에 검은색 굴림체로 크게 박아주세요' 라고 말하는 것 또한 자연언어 기반 마크업 언어라고 할 수 있다.

왜 다양한 언어가 존재할까?
고급언어 & 저급언어 
https://m.blog.naver.com/PostView.nhn?blogId=tipsware&logNo=221041215416&proxyReferer=https:%2F%2Fwww.google.com%2F

 




### 4. GitHub CLI

링크 : https://github.com/KennethanCeyer/tutorial-git#page_with_curl-%EC%86%8C%EC%8A%A4-%EA%B8%B0%EB%A1%9D

*CLI란? 
명령 줄 인터페이스(CLI, command-line interface, 커맨드 라인 인터페이스) 또는 명령어 인터페이스는 가상 터미널 또는 터미널을 통해 사용자와 컴퓨터가 상호 작용하는 방식을 뜻한다. 즉, 작업 명령은 사용자가 컴퓨터 키보드 등을 통해 문자열의 형태로 입력하며, 컴퓨터로부터의 출력 역시 문자열의 형태로 주어진다.




GitHub 명령어 
https://rogerdudler.github.io/git-guide/index.ko.html
제일 퀄리티 높음 :

참고 링크:
https://medium.com/@pks2974/%EC%9E%90%EC%A3%BC-%EC%82%AC%EC%9A%A9%ED%95%98%EB%8A%94-%EA%B8%B0%EC%B4%88-git-%EB%AA%85%EB%A0%B9%EC%96%B4-%EC%A0%95%EB%A6%AC%ED%95%98%EA%B8%B0-533b3689db81

참고 링크:
https://velog.io/@devmin/%EA%B9%83%ED%97%88%EB%B8%8Cgithub-%EB%AA%85%EB%A0%B9%EC%96%B4-%EC%95%8C%EC%95%84%EB%B3%B4%EA%B8%B0
