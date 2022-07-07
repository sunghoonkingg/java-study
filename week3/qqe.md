### 자바가 제공하는 다양한 연산자에 대해 알아봅시다.

### 산술연산자

우리가 알고 있는 일반적인 연산에 사용됩니다. 

사칙연산을 기본으로 하지만 생소한 연산자도 있습니다.

산술연산자는 +, -, *, /, % 5가지로 구성되어있습니다.

나머지 %는 나머지값을 구하는 연산자입니다. 

**예제코드)**

```jsx
public static void 산술연산자() {
    int var1 = 1;
    int var2 = 2;

    System.out.println("var1 + var2 = " + (var1 + var2));
    System.out.println("var1 - var2 = " + (var1 - var2));
    System.out.println("var1 * var2 = " + (var1 * var2));
    System.out.println("var1 / var2 = " + (var1 / var2));
    System.out.println("var1 % var2 = " + (var1 % var2));

    double var3 = 1;
    double var4 = 2;
    System.out.println("var3 / var4 = " + (var3 / var4));
}
```

**결과 값)**

```jsx
var1 + var2 = 3
var1 - var2 = -1
var1 * var2 = 2
var1 / var2 = 0
var1 % var2 = 1
var3 / var4 = 0.5
```

다른 것들은 이해하기 어렵지 않지만 

%가 좀 햇갈립니다. 

5 % 2 이 연산자는 5를 2로 나누었을 때의 

나머지 값을 구하는 연산자입니다. 

그래서 답은 1!

### **비트 연산자(bitwise operator)**

비트 연산자는 비트(bit) 단위로 논리 연산을 할 때 사용하는 연산자입니다.

또한, 비트 단위로 전체 비트를 왼쪽이나 오른쪽으로 이동시킬 때도 사용합니다.

![image](https://user-images.githubusercontent.com/91429710/177756165-0398362a-0aca-45e7-9118-3c7ab3a4fbba.png)

**예제코드)**

```jsx
public static void 비트연산자() {
    /**
     * int 자료형은 8 Byte이므로 32비트로 표현된다.
     * 0000 0000 0000 0000
     * 연산 설명을 편의를 위해 앞의 12자리는 제외하고 실제 값이 표현되는 마지막 4자리만 표현하겠습니다.
     */
    int var1 = 3;  // 0011
    int var2 = 5;  // 0101
    System.out.println("var1 & var2 = " + (var1 & var2));
    System.out.println("var1 | var2 = " + (var1 | var2));
    System.out.println("var1 ^ var2 = " + (var1 ^ var2));
    System.out.println("var1>> = " + (var1 >> 1));
    System.out.println("var1<< = " + (var1 << 1));
}
```

**결과 값)**

```jsx
var1 & var2 = 1
var1 | var2 = 7
var1 ^ var2 = 6
var1 >> = 1
var1 << = 6
```

**AND ( & )**

AND 연산자는 같은 위치의 값 모두 1일 경우에 값이 1이 됩니다.

결과값으로 1 (0001) 이 나옵니다.
![image](https://user-images.githubusercontent.com/91429710/177757433-57628262-58f9-4474-bff7-3240ad1d9537.png)

**OR ( | )**

OR 연산자는 같은 위치의 값 중 하나라도 1일 경우 값이 1이 됩니다.

결과값으로 7  (0001)이 나옵니다.

![image](https://user-images.githubusercontent.com/91429710/177757522-580b7873-4ccd-4b92-b807-78c7132a4aca.png)

**XOR ( ^ )**

XOR 연산자는 같은 위치의 값 중 한개만 1이어야 1이 됩니다.

결과값으로 6 ( 0110 )이 나옵니다.

![image](https://user-images.githubusercontent.com/91429710/177757576-90b10539-59ae-4fea-bc2d-58e533fef754.png)

**Right Shift ( >> )**

Right Shift 연산자는 값을 오른쪽으로 shift 시킵니다.

결과값으로 1이 나옵니다.

![image](https://user-images.githubusercontent.com/91429710/177757645-7e8908ea-f97c-43ba-8c29-583c21b24059.png)

**Left Shift ( << )**

Lift Shift 연산자는 값을 왼쪽으로 shift 시킵니다.

결과값으로 6이 나옵니다.

![image](https://user-images.githubusercontent.com/91429710/177757721-f0d8eafa-6cb5-4d95-afa8-8312b4977a33.png)

### **관계 연산자**

관계 연산자는 양쪽에 있는 데이터를 비교하는 연산자입니다.

![image](https://user-images.githubusercontent.com/91429710/177757902-4b8831db-204f-4545-bdfa-8046caa4f4ff.png)

**예제코드)**

```jsx
public static void 관계연산자() {
    int var1 = 1;
    int var2 = 4;
    Account a = new Account();
    System.out.println("var1 == var2");
    System.out.println(var1 == var2);
    System.out.println("var1 != var2");
    System.out.println(var1 != var2);
    System.out.println("var1 > var2");
    System.out.println(var1 > var2);
    System.out.println("var1 < var2");
    System.out.println(var1 < var2);
    System.out.println("var1 <= var2");
    System.out.println(var1 <= var2);
    System.out.println("var1 >= var2");
    System.out.println(var1 >= var2);
    System.out.println("a instanceof Account");
    System.out.println(a instanceof Account);
}
```

**결과 값)**

```jsx
var1 == var2
false
var1 != var2 
ture
var1 > var2 
false
var1 < var2 
ture
var1 => var2 
false
var1 <= var2 
ture
```
