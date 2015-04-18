## Contents

    

1 개요

2 예제

## 1 개요 ¶

[BASIC](BASIC.md)의 구문 중 하나.

  

[GOTO](%EA%B3%A0%ED%88%AC.md)문과 비슷한 명령문이다. GOTO문과 다른 점이 있다면, 특정 위치로 그냥 넘어가고
마는 게 아니라 RETURN 명령문을 써서 GOSUB문을 어디에 썼든지 그 자리로 복귀시킬 수 있다. 즉, 서브 루틴과 같은 것이다.
그리고, GOTO문에 비해 스파게티 코드가 될 위험이 적다. 서브 루틴이 될 부분을 끝으로 짱박아두면 되니까.

  

GW-BASIC같은 초기 방식에서 많이 썼던 코드로, 구조적 프로그래밍 방식에서는 서브 루틴을 SUB문으로 만들 수 있다. QBASIC의
도움말을 보면 GOSUB문보다 SUB문으로 서브 루틴을 만드는 것이 더 좋다고 나오지만, 경우에 따라서는 GOSUB문으로 서브 루틴을 만드는
게 더 나을 수도 있다.  

## 2 예제 ¶

    
    
    10 FOR I = 1 TO 520   GOSUB 8030 NEXT I40 I = 850 GOSUB 8060 PRINT "메롱"70 END80 PRINT I ^ 290 RETURN

  

이 경우 다음과 같이 나온다.  

  

1  
4  
9  
16  
25  
64  
메롱
