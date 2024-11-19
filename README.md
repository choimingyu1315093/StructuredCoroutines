coroutineScope 와 CoroutineScope는 다르다 (udemy_android Coroutines(구조화) 프로젝트에 해당 내용 있다)

 -> CoroutineScope는 범위를 제공하는 인터페이스고, coroutineScope는 코루틴 빌더(코루틴을 만드는 함수)다.
 
 -> 앱의 생명 주기에 따라 코루틴을 관리할 때 CoroutineScope를 사용한다. (Activity, Fragment, ViewModel 등)
 
 -> coroutineScope는 일시 중단 함수이고, 블록 안에 있는 모든 코루틴이 완료될 때까지 함수는 종료되지 않는다.(구조화된 동시성) 단, 블록 내에서 오류가 발생하면 모두 취소된다. 따라서 블록 내에서 오류가 발생했을 때 안전하게 취소하고 싶을 때 사용한다.
 
 -> 여러가지 코루틴 작업을 할 때 coroutineScope를 사용한다.
