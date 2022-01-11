# 마크다운(Markdown) 문법 정리

### 1. 헤더(Headers) 
    
    # This is H1
    ## This is H2
    ### This is H3
    #### This is H4
    ##### This is H5
    ###### This is H6
    
# This is H1
## This is H2
### This is H3
#### This is H4
##### This is H5
###### This is H6

### 2. 강조(Emphasis)   
#### 2.1. 굵게(Bold)  
```
**Example Bold**  
__Example Bold__  
**Example Bold__ // 다른 기호를 같이 사용하면 표시 불가
```  
**Example Bold**  
__Example Bold__  
**Example Bold__  
  
#### 2.2. 기울임(Italic)  
```
*Example Italic*  
_Example Italic_  
*Example Italic_ // 다른 기호를 같이 사용하면 표시 불가
```  
*Example Italic*  
_Example Italic_  
*Example Italic_  
  
#### 2.3. 굵은 기울임(Bold and Italic)  
```
***Example Bold and Italic***  
___Example Bold and Italic___  
**_Example Bold and Italic_**  
__*Example Bold and Italic*__  
```  
***Example Bold and Italic***  
___Example Bold and Italic___  
**_Example Bold and Italic_**  
__*Example Bold and Italic*__  

#### 2.4. 취소선(Strikethrough)
```
~~Example Strikethrough~~
```  
~~Example Strikethrough~~  
  
### 3. 인용문(Blockquotes) 
#### 3.1. 여러 단락이 있는 인용문
```
> This is a first blockquote.  
>
> This is a second blockquote.  
```  
> This is a first blockquote.  
>
> This is a second blockquote.  

#### 3.2. 중첩된 인용문
```
> This is a first blockquote.  
>> This is a second blockquote.  
>>> This is a third blockquote.  
```  
> This is a first blockquote.  
>> This is a second blockquote.  
>>> This is a third blockquote.  

### 4 코드 삽입
#### 4.1. 인라인 코드 블럭(Inline Code Blocks)
```
`Example`  
```  
`Example`  

#### 4.2. 코드 블럭(Code Blocks)
    ```
    public class Main {
        public static void main (String[] args) {
        	System.out.println("Hello World");
        }
    }
    ```  
```
public class Main {
    public static void main (String[] args) {
      System.out.println("Hello World");
    }
}  
```  
  
    ~~~
    public class Main {
        public static void main (String[] args) {
          System.out.println("Hello World");
        }
    }
    ~~~  
~~~
public class Main {
    public static void main (String[] args) {
      System.out.println("Hello World");
    }
}
~~~  
    ```java // 첫 ``` 옆에 타입 지정 가능(C, Java, xml 등)
    public class Main {
        public static void main (String[] args) {
          System.out.println("Hello World");
        }
    }
    ```  
```java
    public class Main {
        public static void main (String[] args) {
          System.out.println("Hello World");
        }
    }
```  

### 5 리스트(Lists)
#### 5.1. 순서가 있는 리스트  
```
1. list 1  
2. list 2  
0. list 3  
1. list 4  
```  
1. list 1  
2. list 2  
0. list 3  
1. list 4  

#### 5.2. 순서가 없는 리스트  
글머리기호 `*`, `+`, `-` 지원, 혼합사용 가능
```
* list 1
  * list 1-1
    * list 1-1-1  
    
+ list 1
  + list 1-1
    + list 1-1-1  
    
- list 1
  - list 1-1
    - list 1-1-1  
    
* list 1
  + list 1-1
    - list 1-1-1  
    
```  
* list 1
  * list 1-1
    * list 1-1-1  
    
+ list 1
  + list 1-1
    + list 1-1-1  
    
- list 1
  - list 1-1
    - list 1-1-1  
    
* list 1
  + list 1-1
    - list 1-1-1  
    
### 6 줄바꿈
문장 마지막에서 2칸 이상 띄어쓰기

### 7 이미지 삽입
#### 7.1. 인라인 이미지 링크  
```
![coffee](https://cdn.pixabay.com/photo/2021/09/07/10/11/coffee-beans-6603499_960_720.jpg)
```  
![coffee](https://cdn.pixabay.com/photo/2021/09/07/10/11/coffee-beans-6603499_960_720.jpg)


#### 7.2. 참조 이미지 링크  
```
![coffee][image]  

[image]: https://cdn.pixabay.com/photo/2021/09/07/10/11/coffee-beans-6603499_960_720.jpg
```  
![coffee][image]  

[image]: https://cdn.pixabay.com/photo/2021/09/07/10/11/coffee-beans-6603499_960_720.jpg

#### 7.3. 이미지 사이즈 조절  
사이즈 조절 기능은 없기 때문에 `<img width="" height=""></img>`를 이용한다. (px 또는 %로 조절 가능)  
```
<img src="https://cdn.pixabay.com/photo/2021/09/07/10/11/coffee-beans-6603499_960_720.jpg" width="450px" height="300px"></img>  
<img src="https://cdn.pixabay.com/photo/2021/09/07/10/11/coffee-beans-6603499_960_720.jpg" width="40%" height="30%"></img>  
```  
<img src="https://cdn.pixabay.com/photo/2021/09/07/10/11/coffee-beans-6603499_960_720.jpg" width="450px" height="300px"></img>  
<img src="https://cdn.pixabay.com/photo/2021/09/07/10/11/coffee-beans-6603499_960_720.jpg" width="40%" height="30%"></img>  

### 8. 링크(Links)  
#### 8.1. URL 직접 링크
    <http://www.naver.com>  
<http://www.naver.com>  

#### 8.2. 인라인 링크(Inline Links)
    [naver](http://www.naver.com)  
[naver](http://www.naver.com)  

#### 8.3. 참조 스타일 링크(Reference-style Links)
    [homepage][a1]

    [a1]: http://www.naver.com  
[homepage][a1]

[a1]: http://www.naver.com  

### 9. 수평선(Horizontal lines)
```
***
---  // dash(-)  
___  // underscore(_)  
```  
***  
---  
___  

### 10. 토글
```
<details>
<summary>여기를 눌러주세요</summary>
<div markdown="1">       

내용

</div>
</details>
```

<details>
<summary>여기를 눌러주세요</summary>
<div markdown="1">       

내용

</div>
</details>
