---
layout: blog
title: CI /CD production release chain complete!!!
date: 2025-01-11T12:56:41.150-08:00
author: 김승진
tags:
  - 예삶주소록
---
우화 회사에서는 그냥 되 있으니까 이용만 하지

진짜 내가 만들려니 정말 짜증나고 힘드네.

그치만… release-please랑 fly의 기가막힌 tooling으로 

유일하게 나를 귀찮게 한 참으로 짜증난 것은 github이었다.

만약 workflow 를 릴리스플리스에서 이어서 다음 다른 것을 할려고 할 경우

기존의 Github Token가지고는 안된다. 조용히 취소된다.









```
token: ${{ secrets.YOUR_PERSONAL_ACCESS_TOKEN }} 
```

요렇게 해야하고 만드는 PAT는 

read Medadata

read/write: Actions, Content, Pull Request





권한을 줘야 한다.

4시간 헛질 하다가 겨우 해냈다.





하지만 이제는 릴리스 버젼, 자동으로 changelog, main merge하면 staging deploy, 그리고 릴리스 PR 머징하면 production deploy가 이제 가능하다!





prod url: [https://yesalm-prod.fly.dev/](https://yesalm-prod.fly.dev/)





흐유… 이제 도메인 박는 것 남았다.




