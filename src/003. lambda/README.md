# Lambda

저는 간단한 기능(단순 연산 등)은 람다로 정의하고 사용하는 편입니다.

루비에서의 람다는 어떻게 생겼나 궁금했습니다.

람다 선언, 할당 이후 그대로 사용하는 것이 아니라 call을 통해서 call을 해줘야헸습니다.  
Proc를 통해서도 람다와 같은 것을 만들 수 있는데 람다도 inspect를 찍어보니 Proc객체로 나오더군요 ㅇㅅㅇ  
단순 단축 문법(?) 같은 건가 봅니다

물론 전 `Proc.new {}` 같은 방식 보다 `lambda {}` 같은 방식을 쓰겠지만요 둘의 차이를 더 알게된다면 적겠습니당.

// 그리고 몰랐는데 파이썬 람다도 인자 기본값 설정되네요 |ㅅㅇ))