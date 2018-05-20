---
layout: post
title: 왜 파일을 네 개나 건드려야 해?
subtitle: React-redux, redux-saga가 필요한 이유 
category: dev
tags: [web, react, redux, react-redux, dev, saga, redux-saga]
published: true
---
React를 이용해서 웹을 개발한다고 하면, 너무나도 당연하게 redux와 saga를 같이 사용하는 것을 고려한다. 만약 별 생각 없이 redux, saga를 사용해서 request를 보내게 된다면, 다른 프레임워크를 사용할 때보다 훨씬 복잡한 일들을 겪게 된다. 
솔직히, 처음 React, redux, saga를 사용할 떄, _"React는 쓰레기야"_ 라고 생각한 적도 많았다. 고작 request 한 번 받겠다고 파일을 네 개나 건드리는 게 말이나 되나? (정확히는, 4+n이다.) 결국 redux와 saga는, **웹을 하나의 상태로 관리하여 그에 상응하는 이득을 얻는데** 의미가 있다. 즉, redux와 saga는 웹에 불필요한 비용이 될 수 있다. 이 포스트에서는, Redux와 saga를 사용하는 데에서 오는 이점과 단점에 대해 이야기한다.