# 마크다운(Markdown) 문법 정리

## 1. 개요  
### 1.1. Markdown 이란?  
### 1.2. Markdown 장/단점  

## 2. Markdown 사용법(문법)  
### 2.1 헤더(Headers) 
```
# This is H1
## This is H2
### This is H3
#### This is H4
##### This is H5
###### This is H6
```  
# This is H1
## This is H2
### This is H3
#### This is H4
##### This is H5
###### This is H6

### 2.2 글자 강조  
#### 1) 굵게(Bold)  
```
**Example Bold**  
__Example Bold__  
**Example Bold__ // 다른 기호를 같이 사용하면 표시 불가
```  
**Example Bold**  
__Example Bold__  
**Example Bold__  
  
#### 2) 기울임(Italic)  
```
*Example Italic*  
_Example Italic_  
*Example Italic_ // 다른 기호를 같이 사용하면 표시 불가
```  
*Example Italic*  
_Example Italic_  
*Example Italic_  
  
#### 3) 취소선(Strikethrough)
```
~~Example Strikethrough~~
```  
~~Example Strikethrough~~  
  
### 2.3 인용문(Blockquotes) 
```
> This is a first blockquote.  
>> This is a second blockquote.  
>>> This is a third blockquote.  
```  
> This is a first blockquote.  
>> This is a second blockquote.  
>>> This is a third blockquote.  

### 2.4 코드 삽입
#### 1) 인라인 코드 블럭(Inline Code Blocks)
```
`Example`  
```  
`Example`  

#### 2) 코드 블럭(Code Blocks)
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
```java
public class Main {
    public static void main (String[] args) {
    	System.out.println("Hello World");
    }
}
```  

### 2.5 리스트(Lists)
#### 1) 순서가 있는 리스트  
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

#### 2) 순서가 없는 리스트  
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
    
### 2.6 줄바꿈
문장 마지막에서 2칸 이상 띄어쓰기

### 2.7 이미지 삽입
#### 1) 인라인 이미지 링크  
![Alt Text](image_url)  

#### 2) 참조 이미지 링크  
![Alt Text][image]  
[image]: image_url  
