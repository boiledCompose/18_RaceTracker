### 컴포저블에서 suspend function 호출

`LaunchedEffect` 컴포저을은 컴포지션 내에서 제공된 정지 함수를 실행한다. 특징은 다음과 같다.

- `LaunchedEffect()` 컴포저블을 사용하면 컴포저블에서 정지 함수를 안전하게 호출할 수 있다.
- `LaunchedEffect()` 함수가 컴포지션을 시작하면 매개변수로 전달된 코드 블록으로 코루틴이 실행된다.
- 코루틴은 `LaunchedEffect()`가 컴포지션을 종료하면 취소된다. 
