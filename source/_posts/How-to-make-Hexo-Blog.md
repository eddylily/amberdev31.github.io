---
title: 초보인 내가 Hexo 블로그를 만든 과정
date: 2021-12-13 22:52:49
categories: 블로그 개발일지
tags: Hexo
---

</br>

이전에도 블로그를 운영해 본 경험은 많이 있었지만, 이렇게 직접 밑바닥부터(?) 하나하나 쌓아가며 만든 블로그는 여기가 처음이다. 사실 아예 무에서 유를 창조한 것은 아니고, Hexo라는 툴의 도움을 받았다. Hexo가 무엇인지에 대해서는 이미 다른 블로거들이 충분히 설명해두었을 테니, 여기서는 빠르게 여러분이 원하는 본론ー블로그를 설치하는 과정으로 들어가겠다.

<!--more-->
</br>

사실 https://hexo.io/ko/docs/ 에 들어가면 모든 내용이 설명되어 있긴 하다. 영어 독해가 되시는 분은 https://hexo.io/docs/ 를 보셔도 좋다.

필자의 컴퓨터에는 Git이나 Node.js는 이미 설치되어 있었기에 위 문서에서 설명하는 대로 Hexo를 설치하기 위해 곧바로 터미널에 다음과 같이 명령어를 입력했다. 

</br>

    $ npm install -g hexo-cli

</br>

그런데 ERESOLVE 에러가 나며 설치가 되지 않았다. 

[이 블로거](https://sugimotonote.com/2017/10/31/npm-install-error/) 분께서 말씀하시길, Node.js의 버전과 npm의 버전에 따라서 서로 호환이 잘 안 되는 경우가 있다고 한다. 초보자로서 잘은 모르겠지만 그러려니 하며 일단 16.x 버전의 Node.js를 구버전인 12.x 버전으로 다운그레이드하기로 했다.

다음 명령어를 입력하면 기존에 설치된 Node.js의 버전을 v12.18.3으로 다운그레이드할 수 있다.

</br>

    $ npm install -g n
    $ n 12.18.3

</br>

다운그레이드가 잘 되었는지는 다음 명령어를 통해 확인할 수 있다. 자신이 설치하고자 한 버전과 같은 숫자가 뜨면 성공한 것이다. 

</br>

    $ node -v

</br></br>

아무튼 이렇게 해서 Hexo를 설치했다면, 다음은 블로그 환경을 구축할 차례이다. 적당한 곳에 새로운 폴더를 만들고 해당 디렉토리에 들어간 다음, Hexo 블로그 환경을 구축하기 위한 명령어를 입력해준다.

</br>

    $ hexo init hexo
    $ cd hexo
    $ npm install

</br>

첫 번째 명령어는 Hexo의 초기 환경을 세팅하는 명령어이다. 'hexo' 라는 하위 폴더에 필요한 파일들을 설치한다는 의미로 이해하면 된다. 그리고 두 번째 명령어를 입력하여 앞서 만들어진 하위 폴더로 이동한 다음, 세 번째 명령어를 입력하여 Hexo 구동에 필요한 Node 모듈을 설치해주는 것이다. 

위의 과정을 모두 끝마쳤다면 터미널에 다음과 같은 명령어를 입력하여 설치가 잘 되었는지 테스트해보자.
</br>

    $ hexo server

</br>

위의 명령어는 로컬 서버를 가동하는 명령어로, 입력하였을 때 별다른 에러가 발생하지 않는다면 성공한 것이다. 주소창에 'localhost:4000' 을 입력하여 들어가보면 기본 테마가 적용된 Hexo 블로그의 모습이 나타날 것이다.

</br>

    $ hexo server -o
    
</br>

혹은 위와 같이 명령어 뒤에 '-o' 를 붙이면 로컬 서버를 가동시키는 동시에 새 창을 띄워 자신의 블로그 페이지의 모습을 확인할 수 있다. 필요에 따라 두 명령어 중 하나를 사용하면 된다. 

</br></br>

이상으로 기본적인 Hexo 설치 및 블로그 환경 설정 과정을 설명하였다. 다음에는 블로그에 새로운 테마를 적용하고 테마를 수정했던 과정에 대해 포스팅하겠다. 필자는 의외로 이 부분에서 꽤 고생했기 때문에 부디 해당 포스팅이 조금이나마 다른 초보자들에게 도움이 되었으면 좋겠다. 

</br></br>