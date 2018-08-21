---
layout: post
title:  "css 서클 그래프"
date:   2018-08-21 22:09:00 +0900
categories: jekyll update
---

## circleLine
css를 이용한 원형 그래프 구현

약간의 잔머리를 굴렸다.

`svg`나 `canvas`가 아닌 순수 css로만 구현할 수 있을까? 라는 질문에서 시작한 [circleLine](https://github.com/uiwwnw/circleLine)

이전에 찾았던 거지만 border의 그라디언트를 이용하여 그래프를 구현한 소스가 이미존재한다. 하지만 나는 그보다 더 낮은 브라우저에 대응하고 싶었다.

## 원리
1. css2인 clip을 이용한다.
1. 원의 반을 그린다.
1. 그려지기전의 원 그려진 후의 원을 만든다.
1. 총 4개의 반원을 이리저리 이용하여 그림이 그려지는것 처럼 구현한다.
