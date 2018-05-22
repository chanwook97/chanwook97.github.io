---
layout: post
title: 어... 사실 그거 Redux 안 쓰는게 더 나아요.
subtitle: 왜 Redux가 필요하며 Redux를 통해서 무엇을 얻을 수 있을까?
category: dev
tags: [web, react, redux, react-redux]
published: true
---

> 미성숙한 최적화는 악의 근원이다. - [Donald Knuth](https://en.wikipedia.org/wiki/Donald_Knuth)

React와 Redux는 세트다. 너무 같이 붙어다닌다. Redux는 그래서 React가 있는 곳마다 쓰이며 항상, "내가 왜 세 곳의 코드를 건드리면서 Redux를 사용해야 해?"하는 욕을 먹곤 한다. 사실 Redux가 쓸데 없다는 오해를 불러일으키는 이유중 하나는 Redux Tutorial이 단순한 예시를 다루고 있기 때문이다. 