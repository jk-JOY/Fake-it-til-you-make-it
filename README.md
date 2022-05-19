# Fake-it-til-you-make-it
Today I Learn
#2022년 4월 18일
1. 감사를 표현하라
2. 스스로와 동료에게 칭찬하라
3. 스승님께 여쭈어라.
4. 너 스스로를 사랑해라.


그걸 통해서 유니티의 전반적인 

사용법을 익히고 포폴을 준비하면서해당 기술을 활용하는 방법을 배우는것
​
1. 기술의 활용을 통해 필요한 기능을 만들어낼수있다.
2. 그 기술을 코드로 표현해낼때 깔끔하게 표현해낼 수 있다
​

일본어
- 전화회화. 
- 컴퓨터로 쓸 줄 알고. 
​

​

3D_MMORPG
기능관련으로만.
- 서버와 소통하는 API구현
(다듬기 - 디자인패턴)
​

깃 - 협업할때
컨플릭트 났을때 -머지 충돌
리베이스가 무엇인가?
터미널 기준으로 공부
깃메뉴얼이 공짜로 인터넷 체계적으로 공부. 
​
n2까지 3개월. 
​
다작
로직을 외워라. - 그것을 활용하려면
많이 로직을 써봐야한다. 성장속도가 빠른사람. 
​

믿음 
- 목표가 확실함. 
내가 모르는것과 아는것을 확실히 안다.
​
어떻게 어프로지할지?
​

유대인 교육식으로 하브루타 질문으로 접근
스스로에게 끊임없는 질문과 대답
​


# 5.17일 
마크다운으로 깃 작업하는것 배웠다.
"#" 으로 h1 표시
- 표시로 수정

"- - -"  수평선
스페이스바의 4개 == tab키는 다음 줄로
또한 코드조각时 점점점 뒤에 c#명시해주면 해당 언어 활성화 및 함수 색칠!

블록의 인용문구는 >  >  > 표시로 한다

# 5.18일 Collection
Collection에 대해서 배웠다. 
컬렉션은 숫자를 마음대로 넣고 뺄 수 있는 고무줄 상자이다 
컬렉션의 종류로써는 
1. ArrayList
2. List
3. Hashtable
4. Dictionary
5. Queue
6. Stack 
이 있는데 

1.ArrayList는 아무Type도 막 담을 수 있다.

 ``` C# ArrayList arrayList = new ArrayList(); ```   
 
2.List는 특정 자료형 대로만 넣어야한다.

``` C# List<int> list = new List<int>(); ```   
 
3.hashtable은 특정 값을 얻기 위해서는 열쇠가 필요하다
 
``` C# Hashtable hashtable = new Hashtable(); ```   
 
4. Dictionary는 해쉬테이블과 똑같은데, 자료형을 명시해주는것! (arraylist와 list의 유사함과 비슷)
 
``` C# Dictionary<string, int> dictionary = new Dictionary<string, int>(); ```    
  
 
여기까지 보면 서로의 공통점이 보인다. 
 - ArrayList , Hashtable은 박스가 크다. type이 정해진 상태가 아니다.연산에서 불리하다.
 - List와 Dictionary는 타입을 명시한대로 사용해야하기때문에 결과적으로 연산에서 유리하다.

  
  그리고 나머지의 Queue와 Stack이 있다. 
  
5. Queue는 FIFO로써 언큐(in) 디큐(out)으로 존재한다.
  - 특이조건- 조건문에 걸렸기떄문에 쓸대 주의해서 갯수가 있는지 없는지 확인하고 디큐를 해줘야한다.
  ex) 
  ```C#
   Queue<int> queue = new Queue<int>();
  
  void Start(){
  if(Queue.Count != 0)
  {
    Queue.enqueue(5);
    print(Queue.dequeue());
  }
  }
  ```
  
  ```C#     
  
 Stack<int> stack = new Stack<int>();  

   private void Start()
    {
        stack.Push(1);
        stack.Push(2);
    print(stack.Pop());
        if(stack.Count != 0) //하나라도 있을 경우에만 출력!
  }
  ```
   //큐와 스택은 자료형을 명시해줄 수도 있고 안해줘도 된다. 
    //그러나 명시해주는 방향으로 가는게 맞는것 같다, 서로에게 대화가 잘 통해야하니까!
  
  //큐 - 포션제작 대기줄
    //가장먼저 클릭한 포션(가장먼저 제작),    가장 마지막에 클릭된 포션(가장 마지막 제작), 은행대기줄

    //스택 요리게임, 설거지 게임
    // 기존에 쌓여져 있던 그릇들을 치우는데 가장 위에부터 치우는것을 스택




# 5.19일 NameSpace, (Struct+ 생성자 ) Class & Enum
1. nameSpace는 누군가 만들어놓은 것을 쓴다고 생각해야겠다.
-NameSpace를 쓴다는 것은 대형프로젝트, 협업, 외부 라이브러리를 경험하면서 느낄 수 있는데 
이름이 중복될때 문제를 방지하기위해 각각의 NameSpace를 만들고 사용하고 싶은 곳에 직접 선언하여 관리해주는 방법이 있다고 한다.


2. Struct + 생성자 
-struct는 Class와 유사한 점이 많다.
struct는 Legacy선배로써 Class의 형님뻘이다. 
-후배 Class는 상속이 가능하지만, struct는 X , 
-그리고 Class는 변수에 값을 직접 대입해 줄 수 있지만, struct는 불가능하다.(매개변수로써 타Class에서 대입을 해줘야한다.)

-struct는 값 타입,
-Class는 주소 타입이다.

-특이점! Class로 생성할때에는 ```C# Class ~~ = new Class(); ``` 이렇게 해주었지만
Struct는 선언과 동시에 new Class가 처리되기때문에 따로 공간을 만들어주지 않아도 된다!


-생성자는 struct이 직접 값을 대입해주지 못하기때문에 그것을 도와주는 것이 생성자이고 
```C#
public struct Youtube
{
    public int a; 
    public int b; 
    public int c; 
    public int d; 

    //생성자 - 각각 매칭시켜주는것. 
    public Youtube(int _a, int _b, int _c, int _d)
    {
        a = _a; b = _b; c = _c; d = _d;
    }
}

public class StructedTest : MonoBehaviour
{
    int a;
    Youtube keidy = new Youtube(1, 2, 3, 4);
    Youtube keidy2 = new Youtube(5, 6, 7, 8);
}

```
이런 방식으로 사용한다.

3. Enum
-어떤 것을 열거한다는 뜻(넣고 싶은 값을 직접 골라서 사용할 수 있다.)
-특정 조건에 따라서 Enum 값을 사용하는 센스있는 코더로 가까워져 가자!
