# 발표내용 
1. 의식적인 연습이란?     
2. TDD 리팩토링 적용 - 개인   
3. TDD 리팩토링 적용 - 개인(주니어) -> 팀     
4. TDD 리팩토링 적용 - 내가 리더      
    
# 의식적인 연습이란?         
TDD, 리팩토링을 잘 하려면... **연습 연습 연습**               
그런데 무조건 **연습을 많이 한다고 잘할 수 있을까?**            
             
다시 말하자면 우리가 양치를 매일 하는데 양치를 잘 해졌을까?               
**아니다** 우리는 무의식적으로 그저 양치질만 했을 뿐이지 노하우가 좋아지지는 않았다.         
**즉, 우리가 무엇인가를 연습할 때 무조건 많은 시간을 투자한다고 많은 연습을 한다고 역량이 좋아지지는 않습니다.**         
        
박재성 강의자님도 TDD, 리팩토링과 관련해 5-6년을 도전한 후에야          
      
**테스트 하기 쉬운 코드와 테스트하기 어려운 코드를 보는 눈**         
**테스트 하기 어려운 코드를 테스트 하기 쉬운 코드로 설계하는 감(sense)**       
가 생겼다고 한다.       
         
TDD, 리팩토링. 멋져보인다.           
하지만 생각만큼 쉽게 연습할 수 있는 녀석이 아니다.             
**그렇다면 좀 더 효과적으로 연습할 수 있는 방법은 없을까?**    
  
1만 시간의 재발견이란 책에서 아마추어와 프로의 차이는 **목적이 있는 연습** 에 따라 달렸다고 합니다.   

## 의식적인 연습의 7가지 원칙   
1. 효과적인 훈련 기법이 수립되어 있는 기술 연마     
2. **개인의 컴포트 존을 벗어난 지점에서 진행, 자신의 현재 능력을 살짝 넘어가는 작업을 지속적으로 시도**     
3. **명확하고 구체적인 목표**를 가지고 진행       
4. 신중하고 계획적이다. 즉, 개인이 온전히 집중하고 '의식적'으로 행동할 것을 요구   
5. **피드백과 피드백에 따른 행동 변경**을 수반   
6. 효과적인 심적 표상을 만들어내는 한편으로 심적 표상에 의존   
7. **기존에 습득한 기술의 특정 부분을 집중적으로 개선함으로써 발전시키고 수정**하는 과정을 수반 

컴포트 존 즉, 안전지대를 벗어난 지점에서 진행 : 기존 내 방식이 아닌 무언가 새롭게 하고자 하는 방향성 가져야한다.   
   
**의식적인 연습으로 효과적으로 연습하자**   
     
## 의식적인 연습 예시 - 우테코 프리코스      
### 우테코 프리코스 진행 방식       
* 3주 동안 진행 매주 해결해야할 미션을 부여           
* 미션을 완료한 후 GitHub의 Pull Request(이하 PR)로 제출       
* 각 PR 평가 후 공통 피드백      
* 선발 과정이지만 3주 동안 배움이 있는 과정을 만들자     
    
### 1주차 - 프로그레밍 제약사항   
* 자바 코드 컨벤션을 지키면서 프로그래밍한다.   
    * **참고문서** : https://google.github.io/styleguide/javaguide.html 또는 https://myeonguni.tistory.com/1596   
    앞선 문서는 매일매일 읽어도 보람차다 무조건 읽도록  
    * indent(인덴트, 들여쓰기) depth를 3이 넘지 않도록 구현한다. 2까지만 허용한다.   
        * 예를 들어 while문 안에 if문이 있으면 들여쓰기는 2이다.   
        * 힌트 : indent(인덴트, 들여쓰기) depth를 줄이는 좋은 방법은 함수(메서드)를 분리하면 된다.   
    * 함수(메서드)가 한 가지 일만 하도록 최대한 작게 만들어라   

### 1주차 - 피드백  
* space(공백)도 convention 이다.      
    * for, while, if문 사이의 space도 convention이다.     
* 불필요하게 공백 라인을 만들지 않는다.     
    * 공백 라인을 뛰우는 것도 코드상에 문맥이 달라지는 부분에 의도를 가지고 뛰우면 좋겠다.     
* git commit 메시지를 의미있게 작성한다.     
    * git commit 메시지에 해당 commit에서 작업한 내용에 대한 이해가 가능하도록 작성한다.     
    * 10여개의 피드백    
    
### 2주차 - 프로그레밍 제약사항   
* 자바 코드 컨벤션을 지키면서 프로그래밍한다.   
    * **참고문서** : https://google.github.io/styleguide/javaguide.html 또는 https://myeonguni.tistory.com/1596   
    앞선 문서는 매일매일 읽어도 보람차다 무조건 읽도록  
    * indent(인덴트, 들여쓰기) depth를 3이 넘지 않도록 구현한다. 2까지만 허용한다.   
        * 예를 들어 while문 안에 if문이 있으면 들여쓰기는 2이다.   
        * 힌트 : indent(인덴트, 들여쓰기) depth를 줄이는 좋은 방법은 함수(메서드)를 분리하면 된다.   
    * 함수(메서드)가 한 가지 일만 하도록 최대한 작게 만들어라   
* **함수(메서드)의 길이가 15라인을 넘어가지 않도록 구현한다.**  
    * 함수(메서드)가 한 가지 일만 잘 하도록 구현한다.   
* **else 예약어를 쓰지 않는다.**   
    * 힌트 : if 조건절에서 값을 return하는 방식으로 구현하면 else를 사용하지 않아도 된다.   
    * else를 쓰지 말라고 하니 switch/case로 구현하는 경우도 있는데 이같은 경우도 허용하지 않는다.  
    * 자바 코드 컨벤션을 지키면서 프로그래밍한다.     
      
### 2주차 - 피드백  
* **java api를 적극 활용한다.**     
    * 메소드를 직접 구현하기 전에 java api에서 제공하는 기능인지 검색을 해본다.   
       
예시)    
우승자 ```pobi```와 ```jason``` 2명 이상일 때 ```pobi,jason```으로 출력   
   
```java
List<String> winners = Arrays.asList("pobi", "jason");
String result = String.join(",", winners);
```
```java List String combine``` 또는 ```java List String join``` 검색시 알 수 있더라 단순하게 검색하도록   

### 3주차 - 프로그레밍 제약사항   
* 자바 코드 컨벤션을 지키면서 프로그래밍한다.   
    * **참고문서** : https://google.github.io/styleguide/javaguide.html 또는 https://myeonguni.tistory.com/1596   
    앞선 문서는 매일매일 읽어도 보람차다 무조건 읽도록  
    * **indent(인덴트, 들여쓰기) depth를 2가 넘지 않도록 구현한다. 1까지만 허용한다.**
        * 예를 들어 while문 안에 if문이 있으면 들여쓰기는 2이다.   
        * 힌트 : indent(인덴트, 들여쓰기) depth를 줄이는 좋은 방법은 함수(메서드)를 분리하면 된다.
    * **최대한 1을 유지하기 위해 노력하고, 정말 힘든 경우 2까지 허용한다.**
    * 함수(메서드)가 한 가지 일만 하도록 최대한 작게 만들어라   
* **함수(메서드)의 길이가 10라인을 넘어가지 않도록 구현한다.**  
    * 함수(메서드)가 한 가지 일만 잘 하도록 구현한다.   
* **else 예약어를 쓰지 않는다.**   
    * 힌트 : if 조건절에서 값을 return하는 방식으로 구현하면 else를 사용하지 않아도 된다.   
    * else를 쓰지 말라고 하니 switch/case로 구현하는 경우도 있는데 이같은 경우도 허용하지 않는다.  
    * 자바 코드 컨벤션을 지키면서 프로그래밍한다.       
* **함수(메서드)의 인자수를 3개까지만 허용한다. 4개 이상은 허용하지 않는다.**   
    * 클래스를 만들거나 비슷한 작업을 처리하도록 해야겠다.   
    
### 3주차 - 피드백  
* **객체에 메시지를 보내라**   
    * 상태 데이터를 가지는 객체에서 데이터를 꺼내려 (get) 하지 말고 객체에 메시지를 보내라     
   
**미개선 코드**
```java
private boolean isMaxPosition(Car car){
    return car.getPosition() == maxDistance;
}
```
  
**개선 코드**
```java
private boolean isMaxPosition(Car car){
    return car.isMaxPosition(maxDistance); // 오버로딩으로 처리한 것 같다.  
}
```

# 의식적인 연습으로 TDD 리팩토링 적용 - 개인  
TDD 리팩토링 == 운동          
평생동안 연습하겠다는 마음가지음로 시작           
   
## 시작하기 - 주변 정리해 꾸준히 연습할 시간 확보   
* 애인과의 만남 시간 조정   
* 친구들과의 관계 끊기      
* TV 보지 않기, 게임하지 않기      
     
## 시작하기 - 장난감 프로젝트 찾기       
주변 환경에 영향을 받지 않고 꾸준히 연습하기 위함             
회사 프로젝트로는 X -> 회사 프로젝트로 연습하게 되면 언제 어떤 업무가 0순위로 치고 들어올지 모름    
즉, 바빠서 TDD를 못하게되고 리듬이 깨지게 된다.         
      
## 1단계 - 단위테스트 연습   
**내가 사용하는 API 사용법을 익히기 위한 학습 테스트에서 시작**   
* 자바 String 클래스의 다양한 메서드(함수) 사용법        
* 자바 ArrayList에 데이터를 추가, 수정, 삭제하는 방법    
   
**예시**
```java
import org.junit.Test;

import static org.assertj.core.api.Assertions.asserThat;

public class StringTest{
    @Test
    public void split(){
        String[] values = "1".split(",");
        assertThat(values).contains("1");
        value = "1,2".split(",");
        assertThat(values).containsExactly("1", "2");
    }
    
    @Test
    public void substring(){
        String input = "(1,2)";
        String result = input.substring(1, input.length() - 1);
        asserThat(result).isEqualTo("1,2");
    }
}
```
내가 많이 쓰는 메서드가 어떻게 동작하는지 이런 작은 동작부터 하나하나 단위 테스트를 진행해본다.   

**예시2**
```java
import org.junit.Test;

import java.util.ArrayList;

import static org.assertj.core.api.Assertions.asserThat;

public class CollectionTest {
    @Test
    public void arrayList(){
        ArrayList<String> values = new ArrayList<>();
        values.add("first");
        values.add("second");
        assertThat(values.add("thrid")).isTrue();
        assertThat(values.size()).isEqualTo(3);
        assertThat(values.get(0)).isEqualTo("first");
        assertThat(values.contains("first")).isTrue();
        assertThat(values.remove(0)).isEqualTo("first");
        assertThat(values.size()).isEqualTo(2);
    }
}
```
     
### 연습 효과      
* 단위테스트 방법을 학습할 수 있습니다.        
* 단위테스트 도구 (xUnit)의 사용법을 익힐 수 있다.          
* 사용하는 API에 대한 학습 효과가 있다.         
       
내가 구현하는 메서드(함수) 중         
**Input과 Output이 명확한 클래스 메소드(보통 Util 성격의 메서드)** 에 대한 단위 테스트 연습         
        
## 2 단계 - TDD 연습    
어려운 문제를 해결하는 것이 목적이 아니라 TDD 연습이 목적          
**난이도가 낮거나 자신에게 익숙한 문제로 시작하는 것을 추천**       
            
웹, 모바일 UI나 DB에 의존관계를 가지지 않는 요구사항으로 연습한다.       
  
### 문자열 덧셈 계산기 요구사항      
쉼표```,``` 또는 콜론 ```:```을 구분자로 가지는 문자열을 전달하는 경우 구분자를 기준으로 분리한 각 숫자의 합을 반환      

```
입력                  출력  
null or ""  ->          0
"1"         ->          1
"1,2"       ->          3
"1,2:3"     ->          6
```

![TDD](https://user-images.githubusercontent.com/50267433/79682794-2821da80-8260-11ea-87eb-61cd1eef3b80.png)    
   
    
**테스트 코드**   
```java
public class StringCalculatorTest {
    @Test
    public void null_또는_반값() {
        assertThat(StringCalculator.splitAndSum(null).isEqualTo(0));
        assertThat(StringCalculator.splitAndSum("").isEqualTo(0));
    }
    
    @Test
    public void 값_하나(){
        assertThat(StringCalculator.splitAndSum("1").isEqualTo(1));
    }
    
    @Test
    public void 쉼표_구분자(){
        assertThat(StringCalculator.splitAndSum("1,2").isEqualTo(3));
    }
    
    @Test
    public void 쉼표_콜론_구분자(){
        assertThat(StringCalculator.splitAndSum("1,2:3").isEqualTo(6));
    }
}
```

**프로덕션 코드**
```java
public class StringCalculator {
    public static int splitAndSum(String text) {
        int result = 0;
        if (text == null || text.isEmpty()) {
            result = 0;
        } else {
            String[] values = text.split(",|:");
            for(String value : values) {
                result += Integer.parseInt(value);
            }
        }
        return result;
    }
}
```
  
### 3단계 - 메소드 분리 리팩토링      
테스트 코드는 변경하지 말고     
**테스트 대상 코드(프로덕션 코드)를 개선하는 연습을 집중한다.**     
    
**리팩토링 코드**    
```java
public class StringCalculator {
    public static int splitAndSum(String text) {
        if (text==null || text.isEmpty()) return 0;
        String[] values = text.split(",|:");
        return sum(values);
    }
    private static int sum(String[] values){
        int result = 0;
        for(String value : values) {
            result += Integer.parseInt(value);
        }
        return result;
    }
}
```

## 메서드가 한가지 일만 하기  
```java
public class StringCalculator {
    public static int splitAndSum(String text) {
        if (text==null || text.isEmpty()) return 0;
        String[] values = text.split(",|:");
        return sum(values);
    }
    private static int sum(String[] values){
        int result = 0;
        for(String value : values) {
            result += Integer.parseInt(value);
        }
        return result;
    }
}
```
우선 불필요한 변수 사용과 리턴을 배제하였고        
else 구문을 없애며 작업을 처리하도록 했습니다.           
하지만 위 코드도 리펙토링이 잘 되었다 볼수 없습니다.      
    
왜냐하면 ```sum()``` 을 기준으로         
1. 문자열을 숫자로 처리     
2. 숫자를 누적하여 더하기         
   
라는 2가지 작업을 하기 때문입니다.      

```java

public class StringCalculator {
    public static int splitAndSum(String text) {
        if (text==null || text.isEmpty()) return 0;
        String[] values = text.split(",|:");
        int[] numbers = toInts(values);
        return sum(numbers);
    }
    
    private static int[] toInts(String[] values){
        int[] numbers = new int[values.length];
        for(int i=0; i < values.length; i++){
            numbers[i] = Integer.parseInt(values[i]);
        }
        return numbers;
    }
    
    private static int sum(int[] numbers){
        int result = 0;
        for(int number : numbers) {
            result += number;
        }
        return result;
    }
    
}
```   
언뜻보면 코드가 길어진것 같고 for문이 1번에서 2번으로 올라갔지만           
데이터 크기가 크지 않기 때문에 성능에 크게 영향을 미치지 않습니다.             
        
이렇게 메서드가 한가지 일만 처리하게 한다면 이 메소드들이 재활용 될 수 있습니다.                
왜냐하면 가장 작은 단위로 작게 쪼개져있기 때문에 각 추상화 개념에 맞는 경우 사용할 수 있습니다.        
하지만 위와 같이 2가지 추삭적 개념이 존재하면 2가지 개념을 충족시키지 않는다면 재사용이 불가능합니다.     
      
## 로컬 변수가 필요한가?  
```java

public class StringCalculator {
    public static int splitAndSum(String text) {
        if (text==null || text.isEmpty()) return 0;
        String[] values = text.split(",|:");
        int[] numbers = toInts(values);
        return sum(numbers);
    }

    private static int[] toInts(String[] values){
        int[] numbers = new int[values.length];
        for(int i=0; i < values.length; i++){
            numbers[i] = Integer.parseInt(values[i]);
        }
        return numbers;
    }

    private static int sum(int[] numbers){
        int result = 0;
        for(int number : numbers) {
            result += number;
        }
        return result;
    }

}
```
또한 해당 로직에서 로컬변수가 꼭 필요한가 아닌가를 생각을해서 코드를 줄이도록 노력한다.   


**개선 코드**
```java

public class StringCalculator {
    public static int splitAndSum(String text) {
        if (text==null || text.isEmpty()) return 0;
        return sum(toInts(text.split(",|:")));
    }

    private static int[] toInts(String[] values){
        int[] numbers = new int[values.length];
        for(int i=0; i < values.length; i++){
            numbers[i] = Integer.parseInt(values[i]);
        }
        return numbers;
    }

    private static int sum(int[] numbers){
        int result = 0;
        for(int number : numbers) {
            result += number;
        }
        return result;
    }

}
```

## Compose Method 패턴 적용 
메서드(함수)의 의도가 잘 드러나도록 동등한 수준의 작업을 하는 여러 단계로 나눈다. (추상화 레벨을 똑같이해라)     

```java

public class StringCalculator {
    public static int splitAndSum(String text) {
        if (text==null || text.isEmpty()) return 0;
        return sum(toInts(text.split(",|:")));
    }

    private static int[] toInts(String[] values){
        int[] numbers = new int[values.length];
        for(int i=0; i < values.length; i++){
            numbers[i] = Integer.parseInt(values[i]);
        }
        return numbers;
    }

    private static int sum(int[] numbers){
        int result = 0;
        for(int number : numbers) {
            result += number;
        }
        return result;
    }

}
```
같은 경우 ```splitAndSum()```는 다른 두 메서드와 추상화 레벨이 동일하지 않다.    
이유는 이유는 어떻게 계산하는지에 대한 계산식이 보이기 때문이다. -> 추상화 레벨이 올라간다.      
그렇기에 계산식이 보이지 않게끔 해주어 추상화 레벨을 1단계로 낮추어준다.   

**개선 코드**
```java
public class StringCalculator {
    public static int splitAndSum(String text) {
        if (isBlank(text)) return 0;
        return sum(toInts(split(text)));
    }

    private static boolean isBlank(String text){
        return text==null || text.isEmpty();
    }
    private static String[] split(String text){
        return text.split(",|:");
    }

    private static int[] toInts(String[] values){
        int[] numbers = new int[values.length];
        for(int i=0; i < values.length; i++){
            numbers[i] = Integer.parseInt(values[i]);
        }
        return numbers;
    }

    private static int sum(int[] numbers){
        int result = 0;
        for(int number : numbers) {
            result += number;
        }
        return result;
    }

}
```

## 결과

**미 개선 코드**
```java
public class StringCalculator {
    public static int splitAndSum(String text) {
        int result = 0;
        if (text == null || text.isEmpty()) {
            result = 0;
        } else {
            String[] values = text.split(",|:");
            for(String value : values) {
                result += Integer.parseInt(value);
            }
        }
        return result;
    }
}
```

**개선 코드**
```java
public class StringCalculator {
    public static int splitAndSum(String text) {
        if (isBlank(text)) return 0;
        return sum(toInts(split(text)));
    }

    private static boolean isBlank(String text){
        return text==null || text.isEmpty();
    }
    private static String[] split(String text){
        return text.split(",|:");
    }

    private static int[] toInts(String[] values){
        int[] numbers = new int[values.length];
        for(int i=0; i < values.length; i++){
            numbers[i] = Integer.parseInt(values[i]);
        }
        return numbers;
    }

    private static int sum(int[] numbers){
        int result = 0;
        for(int number : numbers) {
            result += number;
        }
        return result;
    }

}
```
이제 두 코드를 살펴보자       
만약 내가 해당 코드및 로직을 알지 못한다는 가정하에 처음 이 코드를 접했다면 어떤 코드가 이해하기 쉬울까?        
단순히 강의에서 말해서가 아니라 객관적으로 2번째 코드가 좋다고 말할 수 있다.          
이유는 1번째는 내가 로직을 하나하나 따라가면서 처리해야하지만         
2번째는 메서드의 이름만 보고도 내가 그 로직을 보지 않더라도 유추가 가능하기 때문이다.        
        
일단 주제인 연습에 관한 결론을 말하자면        
**한번에 모든 원칙을 지키면서 리팩토링하려고 연습하지 마라**           
**한번에 한 가지 명확하고 구체적인 목표를 가지고 연습하라**       
          
연습을 극단적인 방법으로 연습하는 것도 좋다.       
예를 들어 한 메소드 라인 수 제한을 15라인 -> 10 라인으로 줄여가면서 연습하는 것도 좋은 방법이다.         
       
또한 여기서 추가적으로 리팩토링을 하자면 아래와 같습니다.   
 
```java
            numbers[i] = Integer.parseInt(values[i]);
```
여기서도 계산식이 보이므로 관련된 메서드를 만들어줍니다. 

**추가한 메서드**
```java
    private static int toInt(String value){
        int number = Integer.parseInt(value);
        if(number < 0){
            throw new RuntimeException();
        }
        return number;
    }
```

**전체 개선 코드**
```java
 
public class StringCalculator {
    public static int splitAndSum(String text) {
        if (isBlank(text)) return 0;
        return sum(toInts(split(text)));
    }

    private static boolean isBlank(String text){
        return text==null || text.isEmpty();
    }
    private static String[] split(String text){
        return text.split(",|:");
    }

    private static int[] toInts(String[] values){
        int[] numbers = new int[values.length];
        for(int i=0; i < values.length; i++){
            numbers[i] = toInt(values[i]);
        }
        return numbers;
    }

    private static int toInt(String value){
        int number = Integer.parseInt(value);
        if(number < 0){
            throw new RuntimeException();
        }
        return number;
    }

    private static int sum(int[] numbers){
        int result = 0;
        for(int number : numbers) {
            result += number;
        }
        return result;
    }

}
```
이렇게 분리했을 경우 특정 값 처리에 대한 예외처리를 진행할 수 있습니다.            
**그리고 이와 같은 경우 클래스로 분리까지 할 수 있는 확장성 있는 코드가 될 수 있습니다.**              
          
## 리팩토링 연습 - 클래스 분리       
좀전까지는 리팩토링의 메서드 분리였습니다.       
이제 클래스를 만드는 기준으로 클래스를 분리하는 연습을 해보겠습니다.       
     
쉼표```,``` 또는 콜론```:```을 구분자로 가지는 문자열을 전달하는 경우 구분자를 기준으로 분리한 각 숫자의 합을 반환       
**숫자 이외의 값 또는 음수를 전달하는 경우 RuntimeException 예외를 throw 한다**        
  
```
입력                  출력  
null or ""  ->          0
"1"         ->          1
"1,2"       ->          3
"1,2:3"     ->          6
"-1,2:3"    ->          RuntimeException
```

일단 이에 대한 테스트 코드가 추가된다.   

```java
import org.junit.Test;

import static org.assertj.core.api.Assertions.asserThat;

public class StringTest{
    @Test
    public void split(){
        String[] values = "1".split(",");
        assertThat(values).contains("1");
        value = "1,2".split(",");
        assertThat(values).containsExactly("1", "2");
    }
    
    @Test
    public void substring(){
        String input = "(1,2)";
        String result = input.substring(1, input.length() - 1);
        asserThat(result).isEqualTo("1,2");
    }
    
    @Test(expected = RuntimeException.class)
    public void 음수값(){
        StringCalculator.splitAndSum("-1,2:3");
    }
      
}
```

그리고 기존에 리팩토링 했던 코드를 봅시다.   

```java
public class StringCalculator {
    public static int splitAndSum(String text) {
        if (isBlank(text)) return 0;
        return sum(toInts(split(text)));
    }

    private static boolean isBlank(String text){
        return text==null || text.isEmpty();
    }
    private static String[] split(String text){
        return text.split(",|:");
    }

    private static int[] toInts(String[] values){
        int[] numbers = new int[values.length];
        for(int i=0; i < values.length; i++){
            numbers[i] = toInt(values[i]);
        }
        return numbers;
    }

    private static int toInt(String value){
        int number = Integer.parseInt(value);
        if(number < 0){
            throw new RuntimeException();
        }
        return number;
    }

    private static int sum(int[] numbers){
        int result = 0;
        for(int number : numbers) {
            result += number;
        }
        return result;
    }

}
```

### 모든 원시값과 문자열을 포장한다.   
원시값이나 문자열은 이를 포장하는 래퍼 클래스를 만들어서 사용할 수 있습니다.   

```java
    private static int toInt(String value){
        int number = Integer.parseInt(value);
        if(number < 0){
            throw new RuntimeException();
        }
        return number;
    }
```
리턴 하는 값이 원시값이기 때문에 이를 포장하는 래퍼클래스를 만들어보겠습니다.  

```java
public class Positive {
    private int number;
    
    public Positive(String value) {
        int number = Integer.parseInt(value);
        if(number < 0){
            throw new RuntimeException();
        }
        this.number = number;
    }
}
```
그리고 위 코드는 클래스의 특성인 오버로딩을 이용하여 다양하게 구현할 수 있습니다.   

```java
public class Positive {
    private int number;

    public Positive(String value) {
        this(Integer.parseInt(value));
    }

    public Positive(int number) {
        if(number < 0){
            throw new RuntimeException();
        }
        this.number = number;
    }
}
```
**놀라운 점은 오버로딩을 이용해 서로 다른 생성자를 불러서 사용할 수 있다는 점 입니다.**     
그리고 이제 기존 원시값으로 계산되던 형식을 해당 클래스 (Positve)에 맞게 리팩토링해줍니다.   

```java
public class StringCalculator {
    public static int splitAndSum(String text) {
        if (isBlank(text)) return 0;
        return sum(toPositives(split(text)));
    }

    private static boolean isBlank(String text){
        return text==null || text.isEmpty();
    }
    private static String[] split(String text){
        return text.split(",|:");
    }

    private static Positive[] toPositives(String[] values){
        Positive[] numbers = new Positive[values.length];
        for(int i=0; i < values.length; i++){
            numbers[i] = new Positive(values[i]);
        }
        return numbers;
    }

    private static int sum(Positive[] numbers){
        Positive result = new Positive(0);
        for(Positive number : numbers) {
            result = result.add(number);
        }
        return result.getNumber();
    }
}
```
그리고 해당 코드가 돌아가도록 다시 ```Positive``` 클래스에 알맞은 메서드를 구현해주도록 합니다.   

```java
    public Positive add(Positive other){
        return new Positive(this.number + other.getNumber());
    }
    
    public int getNumber(){
        return number;
    }
```

**Positive 개선 코드**
```java
public class Positive {
    private int number;

    public Positive(String value) {
        this(Integer.parseInt(value));
    }

    public Positive(int number) {
        if(number < 0){
            throw new RuntimeException();
        }
        this.number = number;
    }

    public Positive add(Positive other){
        return new Positive(this.number + other.number);
    }

/*
    public Positive add(Positive other){
        return new Positive(this.number + other.getNumber());
    }
*/
    public int getNumber(){
        return number;
    }
}
```

### 클래스 분리 연습을 위해 활용할 수 있는 원칙   
* 일급 콜렉션을 쓴다.    
* 3개 이상의 인스턴스 변수를 가진 클래스를 쓰지 않는다.     
  
일급이란 좀전처럼 int number 라는 한개의 인스턴스 변수를 가지는 객체를 의미하는 것이고     
일급 콜렉션은 콜렉션 자료형을 가지는 인스턴스 변수 한개를 포장하는 클래스를 만들라는 것입니다.          
즉 Set, Map, List와 같은 클래스를 포장하는 클래스를 만들라는 것이며 아래와 같습니다.         
      
```java

import java.util.Set;

public class Lotto {
    private static final int LOTTO_SIZE = 6;
    
    private final Set<LottoNumber> lotto;
    
    private Lotto(Set<LottoNumber> lotto){
        if(lotto.size() != LOTTO_SIZE){
            throw new IllegalArgumentException();
        }
        this.lotto = lotto;
    }
    
}
```

### 3개 이상의 인스턴스 변수를 가진 클래스를 쓰지 않는다.   
말그대로 클래스내의 인스턴스 변수를 3개이상 사용하지 않게끔 만드는 것입니다.    
이게 진짜 어려운 연습입니다.   

```java
public class WinningLotto {
    private final Lotto lotto;
    private final LottoNumber no;
    
    public WinningLotto(Lotto lotto, LottoNumber no){
        if(lotto.contains(no)) {
            throw new IllegalArgumentException();
        }
        this.lotto = lotto;
        this.no = no;
    }
    
    public Rank match(Lotto userLotto){
        int matchCount = lotto.match(userLotto);
        boolean matchBonus = userLotto.contains(no);
        return Rank.valueOf(matchCount, matchBonus);
    }
    
}
```
그리고 이렇게 정량적인 기준으로 연습을 하다보면 ```의식적인 연습```의 사이클로 
나혼자 피드백할 수 있습니다. 예를 들면 else가 있거나 인스턴스변수가 3개 이상이면 잘못된것이지 라고 생각 가능하다.   

## 4단계 - 장난감 프로젝트 난이도 높이기    
점진적으로 요구사항이 복잡한 프로그램을 구현한다.     
앞에서 지켰던 기준을 지키면서 프로그래밍 연습을 한다.     

### TDD 리팩토링 연습하기 좋은 프로그램 요구사항   

* 게임과 같이 요구사항이 명확한 프로그램으로 연습   
* 의존관계(모바일 UI, 웹 UI, 데이터베이스, 외부 API와 같은 의존관계)가 없이 연습  
* 약간은 복잡한 로직이 있는 프로그램  

### 연습하기 좋은 예   
    
* 로또 (단, UI는 콘솔)   
* 사다리 타기 (단, UI는 콘솔)    
* 볼링 게임 점수판 (단, UI는 콘솔)   
* 체스 게임 (단, UI는 콘솔)      
* 지뢰 찾기 게임 (단, UI는 콘솔)       
      
극단적인 연습으로 main 메서드를 돌리지 않고 만들 수 있다면 우리는 경지에 오를 수 있다고 말할 수 있다.     
   
## 5단계 - 의존관계 추가를 통한 난이도 높이기        
웹 UI, 모바일 UI, 데이터베이스와 같은 의존관계 추가         
      
**이때 필요한 역량은**         
테스트하기 쉬운 코드와 테스트하기 어려운 코드를 보는 눈             
테스트하기 어려운 코드를 테스트하기 쉬운 코드로 설계하는 **감(sense)**          
          
앞 단계 연습을 잘 소화했다면 테스트하기 쉬운 코드와 어려운 코드를 분리하는 역량이 쌓였을 것이다.        

## 한 단계 더 나아간 연습  
   
* 컴파일 에러를 최소화하면서 리팩토링하기      
* ATDD 기반으로 응용 애플리케이션 개발하기        
* 레거시 애플리케이션에 테스트 코드 추가해 리팩토링하기 (진짜 어려움)   

### 우리가 TDD 리팩토링 적용이 실패하는 이유     
TDD, 리팩토링 연습이 충분하지 않은 상태에서     
**레거시 애플리케이션에 테스트 코드 추가해 리팩토링하기**      
와 같은 높은 난이도에 바로 도전     

## 구체적인 연습 목표 찾기   
### 객체지향 생활체조 원칙
     
* 규칙 1: 한 메서드에 오직 한 단계의 들여쓰기만 한다.       
* 규칙 2: else 예약어를 쓰지 않는다.        
* 규칙 3: 모든 원시값과 문자열을 포장한다.        
* 규칙 4: 한 줄에 점을 하나만 찍는다.        
* 규칙 5: 줄여쓰지 않는다.(축약 금지)      
* 규칙 6: 모든 엔티티를 작게 유지한다.     
* 규칙 7: 3개 이상의 인스턴스 변수를 가진 클래스를 쓰지 않는다.      
* 규칙 8: 일급 콜렉션을 쓴다     
* 규칙 9: Getter/Setter/Property를 쓰지 않는다.      
    
* 규칙 10: 메소드에서 이상적인 인자 개수는 0개(무항)이다.      
다음은 1개이고 다음은 2개이다. 3개는 가능한 피하는 편이 좋다.      
4개 이상은 특별한 이유가 있어도 사용하면 안된다.       

### TDD 리팩토링 연습을 위해 필요한 것은?     
조급함 대신 **마음의 여유**       
나만의 장난감 프로젝트     
같은 과제를 반복적으로 구현할 수 있는 **인내력, 꾸준력, 성실함**     
          
# TDD 리팩토링 적용 -개인(주니어) => 팀   
TDD, 리팩토링의 필요성을 느꼈다.      
너무 좋다. 팀에 전파하고 싶다.        

## 생각해볼점 
     
* 사람은 기본적으로 변화를 거부하는 성향     
* 팀은 변화를 거부하는 성향이 더 강함      
* 대부분의 사람들은 변화에 실패한 경험을 가지고 있음      
         
## 시작하기       
내가 맡은 기능 구현에 TDD, 리팩토링 적용            
묵묵히 혼자 진행          
          
관심있는 사람이 생기면 전파한다.        
       
내가 구현한 코드 또는 동료의 관심에서 **작은 성공을 맛본다**       
          
리더가 하지 말라고 하면 **그만둔다**      
하지만 나는 많이 성장했기 때문에 갈 곳은 많다.       
걱정하지 마라. 절대 손해 보는 장사는 아니다.      
     
연봉을 올려 이직한다.        
TDD, 리팩토링 전파를 시도한다.      
경력이 쌓이면서 내가 리더가 된다.        
       
# TDD 리팩토링 적용 - 내가 리더    
## '팀에 변화 만들기' 가 더 적합     
### 생각해 볼 점
  
* 사람은 기본적으로 변화를 거부하는 성향     
* 팀은 변화를 거부하는 성향이 더 강함      
* 대부분의 사람들은 변화에 실패한 경험을 가지고 있음         

### 리더가 추가로 생각할 점
     
* 1:1로 공략       
* 팀원이 개선할 부분을 말하고, 해결책을 제안하도록 유도     
   
### 시작하기   
팀원들과의 신뢰 형성이 우선, 1:1 면담을 통해 개선할 부분 찾기    

### 1:1면담에서 한가지만 기억하자   
팀원이 문제점을 이야기할 때     
문제점에 대한 해답을 제시하려하지 말고,        
```어떻게 하면 될까?```, ```너라면 어떻게 할 것 같아?``` 라는 **반문**을 해라       
그 친구들도 문제점을 알고 이를 해결할 방법도 알고 있기에 그런 의견도 들어줘야한다.       
그리고 이런 제안이 리더가 아닌 팀원으로부터 나오게끔 하는 수평적인 문화를 이끌어야 한다.    
       
1:1 면담, 팀 회고를 통해 우선 순위가 높으면서,      
작은 변화를 통해 **가장 높은 효과가 있을 것으로 생각하는 Practice를 선택한다**     
     
선택한 Practice가 개인, 팀 모두 익숙해질 때 까지 **한 가지에 집중**한다.       
       
선택한 Practice로 변화를 완료함으로써 **작은 성공** 맛본다.      
팀이 같이 작은 성공을 맛보는 것이 중요하다.      
       
중요한 것은 어떤 Practice를 하느냐가 아니다.     
현재보다 조금씩 나아지고 있다는 방향성이 중요하다.     
    
# 마치며   
## 작은 성공을 쌓아 큰 성공    
* 장난감 프로젝트로 TDD, 리팩토링 연습해 **작은 성공 맛보기**       
* 내가 구현하는 코드에 한해 TDD, 리팩토링 적용해 **작은 성공 맛보기**    
* 동료에게 짝 프로그래밍 TDD, 리팩토링 경험 전파해 **작은 성공 맛보기**       
* 같이 일하는 주변 사람들에게 변화를 만들어 **큰 성공 맛보기**       

## 실패해도 괜찮다.    
실패하기 전보다는 나는 한 단계 성장한다.   
좋은 회사는 실패해도 같이 도전하는 사람을 원한다.   
실패의 책임을 묻는다면 **그만둔다**   

가장 필요한 것은 가보지 않은 길에 **꾸준히 도전할 수 있는 용기**   
  
