---
layout: post
title: Stable Sort & In-Place
subtitle: 알고리즘 개념
gh-repo: kamja227/kamja227.github.io
gh-badge: [star, fork, follow]
tags: [알고리즘, 정렬, algorithm, sorting, stable_sort, unstable_sort]
comments: true
---

## 안정 정렬 (Stable Sort)

중복된 키를 순서대로 정렬하는 정렬 알고리즘.

    list = [1, 7, 3, 5, 4, 7, 9];
  
이 리스트에서 7이 2번 나온다. 구분을 위해 ()를 이용해 앞의 7은 '7(1)', 뒤에 것은 '7(2)'라고 표시하겠다.
  
    list = [1, 7(1), 3, 5, 4, 7(2), 9];
  
와 같다.

이 리스트를 정렬했을 때,
1.    list = [1, 3, 5, 7(1), 7(2), 9];
2.    list = [1, 3, 5, 7(2), 7(1), 9];

1 처럼 정렬 되는 것을 <u>안정 정렬(Stable Sort)</u> ,
2 처럼 정렬 되는 것을 <u>불안정 정렬(Unstable Sort)</u> 라고 한다.

즉, 정렬 했을 때 중복된 값들의 순서가 변하지 않으면 <u>안정 정렬</u>, 변하면 <u>불안정 정렬</u>인 것이다.

* Stable Sorting Algorithm
  - Insertion Sort
  - Merge Sort
  - Bubble Sort
  - Counting Sort


* Unstable Sorting Algorithm
  - Selection Sort
  - Heap Sort
  - Shell Sort
  - Quick Sort



## In-place Algorithm

In-place 알고리즘이란, 원소들의 개수에 비해서 충분히 무시할만한 저장 공간만을 더 사용하는 알고리즘을 뜻한다.
제자리성(혹은 제자리 정렬)과 같은 의미
일단은 <u>추가적인 메모리 공간이 거의(아예가 아니다) 안 드는 정렬</u>이라고만 알고 있자.


* In-place Sorting Algorithm
  - Insertion Sort
  - Selection Sort
  - Bubble Sort
  - Shell Sort
  - Heap Sort
  - Quick Sort (정의에 따라서 Not in place sorting으로 볼 수도 있으나 흔히 In-place로 본다.)


* Not In-place Sorting Algorithm
  - Merge Sort
  - Counting Sort
  - Radix Sort
  - Bucket Sort


[출처] https://velog.io/@cookncoding/%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98-%EA%B0%9C%EB%85%90-Stable-Sort-Inplace
