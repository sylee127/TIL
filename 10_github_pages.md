# 10_github_pages



# Github pages란?

Github 레포지토리를 이용해서 손쉽게 웹사이트를 배포할 수 있는 기능이다.

보통 자기소개서나 블로그를 운영할 때 많이 사용한다!

더 자세한 정보는 아래 링크를 참고해주세요.

https://pages.github.com/

# 1. 업로드 하고 싶은 홈페이지 코드를 가져온다.

실제로 코드를 작성해도 좋고,(HTML,CSS,JavaScript 활용) 이미 만들어진 코드를 가져와서 변경해도 좋다.

이번 문서에서는 다운 받아서 활용하도록 하겠다.

https://startbootstrap.com/

### 템플릿 다운 받기

Startbootstap → themes 메뉴 → portfolio-resume 메뉴 - CLARENCE TAYLOR - 다운 받기

![pic1](10_github_pages.assets/pic1.png)

![pic2](10_github_pages.assets/pic2.png)

![pic3](10_github_pages.assets/pic3.png)



### 원하는 폴더에 압축을 푼다!

![pic4](10_github_pages.assets/pic4.png)



git bash here 를 이용하거나 macOS의 경우 터미널의 cd 커맨드를 이용해서, 파일이 있는 폴더로 이동한다.

그리고 아래의 명령어를 통해서 commit을 하고 push를 한다.

```jsx
git init
git add .
git commit -m "커밋 메시지"
git remote add origin 레포지토리주소
git push --set-upstream origin master
```



성공했다면 Github 레포지토리에 아래와 같이 출력된다. (파일에 따라 다름)

![pic5](10_github_pages.assets/pic5.png)



### Github - Settings - Pages 클릭

![pic6](10_github_pages.assets/pic6.png)





### 아래처럼 브랜치 선택 후 Save로 저장

![pic7](10_github_pages.assets/pic7.png)





### 아래처럼 뜨면 완료

![pic8](10_github_pages.assets/pic8.png)

![pic9](10_github_pages.assets/pic9.png)





# 추후 수정

vscode에서 `ctrl + f` 찾기 누르고, 왼쪽 화살표 아이콘 누르신다음에 코드 수정하시면 됩니다.

(웹 페이지는 HTML, CSS JavaScript를 활용해서 만듭니다.)

![pic10](10_github_pages.assets/pic10.png)



수정하시고 난 후에는 `git add .`

```
git commit -m "커밋 메시지 작성"
```

`git push` 순서대로 진행하시면 됩니다.