# 구글 면접 준비하기

> * 원문 : [Google Interview University](https://github.com/jwasham/google-interview-university)
* 원저자 : [John Washam](https://github.com/jwasham)
* 번역 : [BayMinimum](https://github.com/BayMinimum)
* 아직 완전히 번역되지 않은 글입니다ㅠ 함께 번역에 참여해 주세요!
## 이 글은...

웹 개발자(독학, 컴공 학위 없음)였던 필자가 구글 소프트웨어 엔지니어가 되기 위한 몇 달 간의 학습 계획이다.

![칠판에 코딩하기 - HBO 실리콘 밸리에서](https://dng5l3qzreal6.cloudfront.net/2016/Aug/coding_board_small-1470866369118.jpg)

이 길고 긴 목록은 **구글 코칭 노트** 에서 가져온 내용과 그 확장으로, 독자 여러분이 꼭 알아야 할 내용들이다.
그리고 면접에 나올 수 있거나 문제를 푸는나 데 도움이 될수 있는 내용들도 아래에 적어 두었다. 많은 항목들은
Steve Yegge의 "[Get that job at Google](http://steve-yegge.blogspot.com/2008/03/get-that-job-at-google.html)" 에서 가져왔으며
구글 코칭 노트의 단어들을 반영하기도 했다.

---

## 목차

- [이 글은...](#what-is-it)
- [존재 이유](#why-use-it)
- [사용 방법](#how-to-use-it)
- [구글구글 하게 해줄게](#get-in-a-googley-mood)
- [필자는 취직했나요?](#did-i-get-the-job)
- [저와 함께 가요!](#follow-along-with-me)
- [당신은 멍청하지 않습니다](#dont-feel-you-arent-smart-enough)
- [구글에 대해](#about-google)
- [영상 자료에 대해](#about-video-resources)
- [면접 과정 & 면접 준비 전반](#interview-process--general-interview-prep)
- [면접을 위한 언어 하나 선택](#pick-one-language-for-the-interview)
- [시작하기 전에...](#before-you-get-started)
---

## 존재 이유

나는 이 계획을 따르면서 구글 면접을 준비하고 있다. 컴퓨터 공학 전공이 아닌, 경제학 학위 소지자인 나는 1997년부터 웹, 서비스를 구축하고 스타트업을 시작해 왔다. 여기까지 매우 성공적인 길을 걸어왔지만, 구글에서 일하고 싶었다. 더 큰 생태계에서, 컴퓨터 시스템, 알고리즘 효율성, 데이터 구조 성능, 저수준 언어를 비롯하여 이것들이 어떻게 동작하는지를 제대로 이해하고 싶었다. 만약 독자 여러분이 이것들에 대해 아무것도 모른다면, 구글은 여러분을 채용하지 않을 것이다.

내가 이 프로젝트를 시작했을 때는, 스택이나 힙 같은건 몰랐고, Big-O, 트리에 대해서도 몰랐으며, 그래프 순회를 할 줄도 몰랐다. 만약 내가 정렬 알고리즘을 짜야 했다면, 분명히 영 좋지 못했을 것이다. 내가 써본 데이터 구조는 전부 언어에 내장된 것뿐이었고, 그것들이 실제로 어떻게 작동하는지는 전혀 알지 못했다. 메모리 관리 따위는 프로세스가 "메모리 부족" 에러를 띄우지 않는 이상 할 필요도 없었다. 지금까지 나는 약간의 다차원 배열과 몇천개의 연관 배열은 사용해 보았지만, 데이터 구조를 바닥부터 짜 본 적은 한 번도 없었다.

하지만 이 계획을 따라 공부한 후에는 내가 채용될 것이라는 자신감을 가지고 있다. 긴 계획이다. 몇 달이 걸릴 것이다. 만약 독자 여러분이 이미 이런 것들에 익숙하다면 훨씬 적은 시간이 걸릴 것이다.

## 사용 방법

아래의 개요에 따라 순서대로 진행하면 된다.

나는 작업 목록으로 항목 체크를 지원하는 GitHub식 마크다운을 사용하고 있다.

- [x] 항목들에 체크할 수 있도록 새로운 branch를 만들고, 대괄호 사이에 x를 넣어 체크하면 된다. : [x]


    새로운 branch를 포크하고 아래 명령을 입력하자.

`git checkout -b progress`

`git remote add jwasham https://github.com/jwasham/google-interview-university`

`git fetch --all`

    마친 항목들에 x표시를 한 후

`git add . `

`git commit -m "Marked x" `

`git rebase jwasham/master `

`git push --force `

[GitHub식 마크다운에 대해 더 알아보기](https://guides.github.com/features/mastering-markdown/#GitHub-flavored-markdown)

## 구글구글 하게 해줄게

"[미래의 구글러 마크](https://github.com/jwasham/google-interview-university/blob/master/extras/future-googler.pdf)"를 한두장 인쇄하여 주변에 붙여두고 항상 바라보자.

[![미래의 구글러 마크](https://dng5l3qzreal6.cloudfront.net/2016/Oct/Screen_Shot_2016_10_04_at_10_13_24_AM-1475601104364.png)](https://github.com/jwasham/google-interview-university/blob/master/extras/future-googler.pdf)

## 필자는 취직했나요?

아직 지원하지 않았습니다.

지금 당장은 붙잡고 있는 프로그래밍 문제가 있습니다. 몇 주 후에 이 문제를 해결하고 나서, 2월부터 계속 붙잡고 있던 추천인을 통해 지원할 것입니다.

    추천해줘서 고마워요, JP.

## 저와 함께 가요!

저도 가는 중입니다. 제 블로그 ([GoogleyAsHeck.com](https://googleyasheck.com/))에서 함께 가요!

- 트위터: [@googleyasheck](https://twitter.com/googleyasheck)
- 트위터: [@StartupNextDoor](https://twitter.com/StartupNextDoor)
- 구글+: [+Googleyasheck](https://plus.google.com/+Googleyasheck)
- 링크드인: [johnawasham](https://www.linkedin.com/in/johnawasham)

![John Washam - Google Interview University](https://dng5l3qzreal6.cloudfront.net/2016/Aug/book_stack_photo_resized_18_1469302751157-1472661280368.png)

## 당신은 멍청하지 않습니다
- 구글에서 일하는 엔지니어들은 분명 똑똑하지만, 꼭 구글에서 일한다고 해서 우리가 생각하는 것만큼 똑똑하지는 않을 수도 있어요!
- [천재 프로그래머에 대한 오해](https://www.youtube.com/watch?v=0SARbwvhupQ)

## 구글에 대해

- [ ] 학생들을 위해 - [Google Careers: Technical Development Guide](https://www.google.com/about/careers/students/guide-to-technical-development.html)
- [ ] 검색의 동작원리:
    - [ ] [검색의 진화(영상)](https://www.youtube.com/watch?v=mTBShTwCnD4)
    - [ ] [검색의 원리-이야기](https://www.google.com/insidesearch/howsearchworks/thestory/)
    - [ ] [검색의 원리](https://www.google.com/insidesearch/howsearchworks/)
    - [ ] [검색의 원리 - Matt Cutts (영상)](https://www.youtube.com/watch?v=BNHR6IQJGZs)
    - [ ] [구글은 어떻게 검색 알고리즘을 개선하는가 (영상)](https://www.youtube.com/watch?v=J5RZOU6vK4Q)
- [ ] 시리즈:
    - [ ] [구글 검색은 어떻게 모바일을 다뤘는가](https://backchannel.com/how-google-search-dealt-with-mobile-33bc09852dc9)
    - [ ] [우리의 필요사항을 찾기 위한 구글의 비밀 연구](https://backchannel.com/googles-secret-study-to-find-out-our-needs-eba8700263bf)
    - [ ] [구글 검색은 당신의 다음 뇌가 될 것이다](https://backchannel.com/google-search-will-be-your-next-brain-5207c26e4523)
    - [ ] [데미스 하사비스의 Deep Mind](https://backchannel.com/the-deep-mind-of-demis-hassabis-156112890d8a)
- [ ] [책: 구글은 어떻게 일하는가](https://www.amazon.com/How-Google-Works-Eric-Schmidt/dp/1455582344)
- [ ] [Made by Google 발표 - 2016/10 (영상)](https://www.youtube.com/watch?v=q4y0KOeXViI)

## 영상 자료에 대해

몇몇 영상은 MOOCs라 불리는 Coursera, EdX, or Lynda.com 강의를 수강해야만 볼 수 있다.
가끔씩은 강좌가 아직 열리지 않아 영상을 보지 못하고, 두 달 정도 기다려야 할 때도 있다. Lynda.com 강좌는 무료가 아니다.

    강좌 동영상과 함께 사용할 수 있는, 언제나 공개되어 있는 무료 영상(유튜브 등)을 찾아주시면 감사하겠습니다.
    저는 대학 강좌 동영상을 사용하길 좋아합니다.

## 면접 과정 & 면접 준비 전반

- [ ] 영상:
    - [ ] [구글에서 일하는 방법: 후보자를 위한 도움말 (영상)](https://www.youtube.com/watch?v=oWbUtlUhwa8&feature=youtu.be)
    - [ ] [구글 면접자들이 밝히는 기술적 면접 팁 (영상)](https://www.youtube.com/watch?v=qc1owf2-220&feature=youtu.be)
    - [ ] [구글에서 일하는 방법: 기술 이력서 준비하기 (영상)](https://www.youtube.com/watch?v=8npJLXkcmu8)

- [ ] 읽을거리:
    - [ ] [구글러가 되기 위한 3단계](http://www.google.com/about/careers/lifeatgoogle/hiringprocess/)
    - [ ] [구글 일자리를 얻자](http://steve-yegge.blogspot.com/2008/03/get-that-job-at-google.html)
        - 위 글에 제시된 독자 여러분이 알아야 할 모든 것들은 이 글 아래에 수록되어 있다.
    - [ ] _(상당히 오래됨)_ [구글에 일자리를 가지는 방법, 면접 질문, 채용 과정](http://dondodge.typepad.com/the_next_big_thing/2010/09/how-to-get-a-job-at-google-interview-questions-hiring-process.html)
    - [ ] [전화 면접 질문](http://sites.google.com/site/steveyegge2/five-essential-phone-screen-questions)

- [ ] 준비 강좌:
    - [ ] [소프트웨어 엔지니어 면접에 관한 모든것](https://www.udemy.com/software-engineer-interview-unleashed):
        - 전 구글 면접관으로부터 배우는 소프트웨어 엔지니어 면접을 준비하는 방법

- [ ] 추가 (구글 권장사항 아님, 필자의 추가):
    - [ ] [ABC: Always Be Coding](https://medium.com/always-be-coding/abc-always-be-coding-d5f8051afce2#.4heg8zvm4)
    - [ ] [학위 없이 구글에 들어가기 위한 4단계](https://medium.com/always-be-coding/four-steps-to-google-without-a-degree-8f381aa6bd5e#.asalo1vfx)
    - [ ] [화이트보딩](https://medium.com/@dpup/whiteboarding-4df873dbba2e#.hf6jn45g1)
    - [ ] [구글은 고용, 관리, 문화에 대해 어떻게 생각하는가](http://www.kpcb.com/blog/lessons-learned-how-google-thinks-about-hiring-management-and-culture)
    - [ ] [프로그래밍 면접에서의 효과적인 화이트보딩](http://www.coderust.com/blog/2014/04/10/effective-whiteboarding-during-programming-interviews/)
    - [ ] 코딩인터뷰 완전 분석 Set 1:
        - [ ] [게일 L. 맥도웰 - 코딩인터뷰 완전 분석 (영상)](https://www.youtube.com/watch?v=rEJzOhC5ZtQ)
        - [ ] [저자 게일 라크만 맥도웰과 함께하는 코딩인터뷰 완전 분석 (영상)](https://www.youtube.com/watch?v=aClxtDcdpsQ)
    - [ ] 빅 4에서 일자리 얻기:
        - [ ] [''빅 4에서 일자리 얻기 - 아마존, 페이스북, 구글, 마이크로스프트'' (영상)](https://www.youtube.com/watch?v=YJZCUhxNCv8)
    - [ ] [구글 면접 탈락기](http://alexbowe.com/failing-at-google-interviews/)

## 면접을 위한 언어 하나 선택

이에 대해 쓴 짧은 글: [중요: 구글 면접을 위한 언어 하나 선택](https://googleyasheck.com/important-pick-one-language-for-the-google-interview/)

코딩 면접에서는 본인에게 잘 맞는 어떤 언어든 사용할 수 있지만, 일반적으로 다음 언어들이 정형화된 선택이라 할 수 있다:

- C++
- Java
- Python

다음 언어들도 사용할 수는 있지만, 약간의 주의 사항이 따를 수 있다:

- JavaScript
- Ruby

독자 여러분은 선택한 언어를 매우 편안하게 사용할 수 있어야 하고, 그 언어에 대한 지식이 풍부해야 한다.

선택에 대한 더 읽을거리:
- http://www.byte-by-byte.com/choose-the-right-language-for-your-coding-interview/
- http://blog.codingforinterviews.com/best-programming-language-jobs/
- https://www.quora.com/What-is-the-best-language-to-program-in-for-an-in-person-Google-interview

[언어 관련 자료](programming-language-resources.md)

필자 또한 배우고 있는 입장이기 때문에, 이 글에는 C, C++, Python을 배우는 내용도 약간 포함되어 있다. 사용된 책들을 보려면 맨 아래를 보자.
