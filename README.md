# Typescript-challenge
노마드코더 타입스크립트 챌린지 (2주)
# Typescript

## 타입스크립트 사용 이유

> **타입 안정성** 때문
> 

### JS의 타입 불안정성

- 에러를 보여주기 않기 위해 개떡같이 코딩해도 찰떡같이 나와버림
- 런타임 에러 : 콘설 안의 에러 / 코드가 실행되면서 비로소 에러를 알게 됨

# 타입스크립트

> strongly typed programming
> 
- 타입스크립트로 작성한 코드 → JS로 생성됨(브라우저에서 JS로 컴파일됨)
    
    (브라우저가 타입스크립트를 JS로 이해, node는 둘다 각각 수용)
    
- 타입스크립트의 보호장치는 JS로 변환되기 전 실행됨
    - 타입스크립트 코드에 에러가 있으면, JS로 컴파일되지 않음(보호장치)
    - 코드를 실행시키기 전에 에러가 있다고 알려줌

### 타입 지정

1. **데이터와 변수의 타입을 명시적으로 정의**
    
    ```tsx
    let a = "hello"
    let b : boolean = false
     <!-- : boolean이 ts 방식 - type checker가 타입 확인해줌 -->
    let c : number[] = []
    c.push(1)
    const player = {
    	name : "jiwon"
    }
    ```
    
2. **JS처럼 변수만 생성 → TS가 타입 추론해줌**
    
    ```tsx
    let a = "hello"
    a = "bye"
    <!-- string을 string으로 바꿨기 때문에 괜찮음 -->
    ```