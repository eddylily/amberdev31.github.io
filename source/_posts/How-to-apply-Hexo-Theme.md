---
title: 초보인 내가 Hexo 블로그를 만들며 겪은 우여곡절
date: 2021-12-24 10:51:57
categories: 블로그 개발일지
tags: Hexo
---
</br>

테마를 설치했다면 이제는 적용해 볼 차례이다. 여기서 필자는 꽤나 많이 애를 먹었다. 총 3번의 실패를 겪었고, 결국은 가장 대중적으로 쓰이는 icarus라는 테마에 일단은 정착하기로 했다. 실패의 과정에 대해서는 이어서 간단히 서술하겠다.

<!-- more -->

</br>

### 'Hexo not found' 에러

</br>

엊그제까지만 해도 잘 구동되던 Hexo가 어느 날 갑자기 먹통이 되었다. 아무리 Hexo 관련 명령어를 터미널에 입력해보아도 Hexo를 찾을 수 없다는 에러 메시지만이 나를 맞이했다. 

</br>

    $ npm config set prefix /usr/local
    
</br>

내용을 입력하세요.

</br>

### Claudia 테마

</br>

디자인도 마음에 들었고 처음에 딱 꽂혔던 테마였다. 그런데 이 테마는 딸려오는 플러그인이 너무 많았다. 그 중에서 sass 플러그인이 필자의 컴퓨터와 계속해서 충돌을 일으켜서 결국 적용을 포기했다.

</br>

### Anisina 테마

</br>

그래서 이번에는 가급적 추가적인 플러그인 설치가 필요치 않은 테마를 찾아보기로 했다. 그렇게 발견한 것이 이 테마다. 그런데 초보자가 뜯어고치기에는 너무나 어려운 구조로 되어 있었다. 그래서 결국 이 테마도 포기했다. 

</br>

### Icarus 테마

구글링만 해 봐도 알 수 있듯이, Hexo로 구축된 블로그에서 가장 대중적으로 쓰이는 테마이다. 생김새도 무난하며 디자인을 수정하기도 쉬운 편이다. 수정하다 막히는 부분이 생겨도 구글링하면 어지간하면 다 나온다. 한국어로 설명된 자료도 많은 편이라 굳이 영어나 일본어로 적힌 블로그까지 찾아보지 않아도 괜찮았다.