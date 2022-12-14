# 베이즈 정리(bayes theorem)

어떤 사건이 서로 배반하는 원인 둘에 의해 일어난다고 할 때 실제 사건이 일어났을 때 이것이 두 원인 중 하나일 확률을 구하는 정리를 베이즈정리라고 한다.

식은 아래와 같이 표현된다.  
$P(B∣A)=(P(A∣B)P(B))/P(A)$

머신러닝에서는 관찰결과를 토대로 사후확률을 계속 업데이트하는 부분에서 베이즈 정리를 활용한다.

링크에서 다룬 하나의 확률실험을 가지고 그대로 이어서 작성해보려고한다.
https://github.com/platypus46/Statistics_InformationTheory/blob/main/probability_foundation.ipynb

실험을 토대로 아래의 식을 서술하면 "하얀공이 나왔다는 사실만 알고 어느 병에서 이 공이 나왔는지는 모른다. 이 공이 나온 상자번호를 추정하라"로 표현 할 수 있다.  
$b=argmaxP(B|A)$

이에 베이즈 정리를 적용하면  
$P(1|하얀색)=(P(하얀색|1)P(1))/P(하얀색)=9/43$  
$P(2|하얀색)=(P(하얀색|2)P(2))/P(하얀색)=16/43$  
$P(3|하얀색)=(P(하얀색|3)P(3))/P(하얀색)=18/43$  ←3번 박스일 확률이 가장높음
<br/>  
$P(B∣A)=(P(A∣B)P(B))/P(A)$  
위의 식에 대응해서 해석해보면  
P(B∣A)←사후(posterior)확률  
P(A∣B)←우도(likelihood)확률  
P(B)←사전(prior)확률  

베이즈정리는 사후확률=우도확률*사전확률로 표현한 것이라고 할 수 있다.


### 최대우도
매개변수(모수)를 모르는 상황에서 매개변수를 추정하는 문제에서 활용되는데 확률변수에서 관찰된 값을 토대로 확률변수의 매개변수를 구하는 방법을 말한다.  

$ ^Θ=arg maxP(X|Θ)$

**유튜브 둘러보다가 베이즈정리에 대해 이해하기 쉽게 설명해줘서 추가**  
https://www.youtube.com/watch?v=Y4ecU7NkiEI
