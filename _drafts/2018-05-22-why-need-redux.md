---
layout: post
title: 어... 사실 그거 Redux 안 쓰는게 더 나아요.
subtitle: 왜 Redux가 필요하며 Redux를 통해서 무엇을 얻을 수 있을까?
category: dev
tags: [web, react, redux, react-redux]
published: true
author: Chanwook Kim
---

# 서론
React를 사용한지 약 1~2년 정도 된 저는 처음에 React에 대해 충분한 경험을 쌓기 전에 Redux를 배웠습니다. 실제로 대부분
React와 Redux는 세트다. 너무 같이 붙어다닌다. Redux는 그래서 React가 있는 곳마다 쓰이며 항상, "내가 왜 세 곳의 코드를 건드리면서 Redux를 사용해야 해?"하는 욕을 먹곤 한다. 사실 Redux가 쓸데 없다는 오해를 불러일으키는 이유중 하나는 Redux가 남용되고 있기 때문이다. 이 글에서는 **Redux는 React에 왜 필요한지, Redux를 통해서 무엇을 얻을 수 있을 지**에 대해 다뤄보고자 한다.

# Redux의 철학
- 어플리케이션의 상태를 단순한 Object로 표현한다.: 스토어
- 어플리케이션의 상태 *변화* 를 단순한 Object로 표현한다.: 액션
- Describe the logic for handling changes as pure functions.: 리듀서


# 왜 React만으로는 부족하고 Redux가 필요한가?
중앙에서 state를 관리하기 위해.
https://medium.com/dailyjs/when-do-i-know-im-ready-for-redux-f34da253c85f

# Redux를 통해 무엇을 얻을 수 있을까?

## 중앙에서 정보를 관리할 수 있다.(uni-directional)

- 예시1: auth 정보.
- 예시2: normalized data
- 예시3: modal open close


## action: 앱의 상태가 변화하는 것을 간단한 Object로 표현한다.
- undo, redo histories 관리.

## store: 앱의 상태를 간단한 Object로 표현한다.
- 디버깅의 용도로 사용한다.
- 서버에 저장해서 다시 Load해서 어디서든 사용할 수 있게 하자.


### Summaries

w
### 참고 자료
- [You may not need redux](https://medium.com/@dan_abramov/you-might-not-need-redux-be46360cf367): Redux 개발자가 이야기하는, 왜 Redux가 필요한지.
- [When do I know I'm ready for redux?](https://medium.com/dailyjs/when-do-i-know-im-ready-for-redux-f34da253c85f): Redux가 왜 필요한지에 대해, 움짤과 함께 설명하는 명쾌한 포스트.