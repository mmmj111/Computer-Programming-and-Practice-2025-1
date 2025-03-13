# 함수선언 (매개변수리스트가 있을 때)

매개변수는 함수가 호출될 때마다 메모리 공간을 새로 할당받고 함수 실행을 종료할 때 삭제됩니다. 
매개변수의 초기값은 호출할 때 정한 값입니다. 
함수 선언은 함수의 이름, 반환타입, 매개변수의 타입을 정합니다.  
함수 선언시 매개변수의 이름은 적지 않고 타입만 적어도 됩니다. 
매개변수가 없는 함수를 선언할 때는 괄호 안에 void만 적습니다. 

`타입` `이름` `(` `매개변수리스트` `)` `;` 형태로 함수선언을 합니다.

`매개변수리스트`는 `매개변수선언` 또는 `매개변수리스트` `,` `매개변수선언` 입니다. 

`매개변수선언`은 `타입` `이름` 또는 `타입` 입니다. 

#### 코드 예시:
```c
int f(int, int); /* 반환 타입이 int고, 이름이 f고, 매개변수 두개의 타입이 모두 int인 함수의 선언 */
int g(int a, int b); /* 이름이 g고, 함수 종류는 f와 동일한 함수의 선언 */
int h(void); /* 반환 타입이 int고, 이름이 h고, 매개변수가 없는 함수의 선언 */
int x(); /* 반환 타입이 int고, 이름이 x고, 매개변수에 대해서는 정하지 않은 함수의 선언 */
```

### 관련 C 표준
3.5.4.3 Function declarators (including prototypes)
> Semantics
> 
> A parameter type list specifies the types of, and may declare identifiers for, the parameters of the function.
> ... The special case of void as the only item in the list specifies that the function has no parameters.

3.5 DECLARATIONS
> Constraints
>
> All declarations in the same scope that refer to the same object or function shall specify compatible types.

3.5.4.3 Function declarators (including prototypes)
> Semantics
>
> For two function types to be compatible, both shall specify compatible retury types.
> Moreover, the paremeter type lists, ... , shall agree in the number of parameters ... ;
> corresponding parameters shall have compatible types. ...
