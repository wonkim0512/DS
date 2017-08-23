# Abstract Data Structures

An abstract data type (ADT) is a mathematical model for a certain class of data structures that have similar behavior. Different classes of abstract data types have many different but functionally equivalent data structures that implement them.

Data structures can be classified as either contiguous (composed of single slabs of memory) or linked (distinct chunks of memory bound together by pointers). In Python, contiguously-allocated structures include strings, lists, tuples, and dictionaries.

In the following sections we will learn how to write abstract data structures, whose can either use Python’s builtin contiguous structures or be made of pointers.

자료 자체의 형태와 그 자료에 관계된 연산들을 수학적으로만 정의한 것. 따라서 대수학이 다루는 대수적 구조로 볼 수도 있으며, 자료구조가 포함하는 구현 세부사항은 전혀 정의하지 않는다. 

스택을 예로 들면, 스택의 형태는 삽입한 순서대로 쌓이는 값들의 모임이고, 스택의 제일 위에 값을 넣는 push연산과 스택 제일 위의 값을 하나 빼서 알려주는 pop연산이 있다고 할 수 있다. 여기에 필요하다면 스택이 비었는지 알아보는 empty연산, 스택에 쌓인 값이 몇 개인지 알아보는 size연산을 정의할 수도 있다.

이 때, 스택이 내부적으로 배열로 구현되는지 연결 리스트로 구현되는지, size연산을 수행할 때 원소의 개수를 일일히 세는지 아니면 개수를 따로 저장해두는지와 같은 세부사항들은 추상적 자료형에서는 다루지 않으며, 그걸 다루기 시작하면 자료구조의 영역으로 넘어가게 된다. 다만, 경우에 따라 알고리즘에서 요구하는 계산 복잡도, 즉 push연산이 O(1)인지 O(n)인지와 같은 부분을 추가로 다룰 수도 있다.

객체 지향 프로그래밍에서의 클래스의 개념과 일맥상통한다고 볼 수도 있다. - [추상적 자료형 by 나무위키](https://namu.wiki/w/%EC%B6%94%EC%83%81%EC%A0%81%20%EC%9E%90%EB%A3%8C%ED%98%95)
