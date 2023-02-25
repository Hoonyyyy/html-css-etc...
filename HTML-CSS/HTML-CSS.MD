# HTML 기초 시작

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
띄어쓰기를 &nbsp; 하고싶다.<br/> 그리고<br/>
줄바꿈을<br/>
하고싶다
</body>
</html>
~~~

- br/ : 줄바꿈
- &nsp : 띄어쓰기



### 레이아웃을 위한 div, span 태그 ( div는 포장박스, span은 포장지)

#### div
- divsion 약자
- 뜻 그대로 콘텐츠의 영역을 나눠주고 레이아웃을 만드는 데에 아주 중요한 역할을 함
- div는 기본값으로 너비를 100% 가지고 있는 것이 특징
- div 여러개 만들고 30% 하더라도 한 줄에 이어지는것이 아닌 한 줄씩 차지함
- 조심하기

#### span
-  글을 이어 붙여서 쓰는 것처럼 너비가 넘어가지 않는 이상, 계속 이어서 붙일 수 있는 특징을 가지고 있음

--------------------------------------------------------------------------------------------------------------


# CSS 기초 시작
- css는 html의 시각적인 것을 구현해 주는 언어
- ***시각*** 이기에 디자이너에게 매우 중요함
- 기본적으로 style ~ /style 이라는 태그 안에 입력 해야함

### css는 기본적으로 선택자(selector), 속성(property), 값(value)로 구성되어 있음 그리고 값 뒤에 항상 세미콜론(;) 붙음


### 맥에서 한글 안깨지게 하려는 코드
~~~html
<meta charset="utf-8">
~~~


### class 이용 색을 다르게 이용하고 싶을때
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>Title</title>
        <style>
            
            .hello1 {
                color: blue;
            }

            .hello2 {
                color: black;
            }



        </style>
    </head>
    <body>
        <div class = "hello1">안녕하세요.</div>
        <div class="hello2">안녕하세요.2</div>
        <div class = "hello1">안녕하세요.3</div>
        <div class="hello2">안녕하세요.4</div>
        <div class = "hello1">안녕하세요.5</div>
        <div class="hello2">안녕하세요.6</div>
    </body>
</html>
```


### style에서 지정하면 body부분에서 가져와서 쓸수 있구나
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>Title</title>
        <style>

            .hello1 {
                color: black;
            }

            .hello2 {
                color: brown;
            }

            .text_bold {
                font-weight: bold;
            }


        </style>
    </head>
    <body>
        <div class="hello1">안녕하세요.</div>
        <div class="hello2">안녕하세요.2</div>
        <div class="hello1">안녕하세요.3</div>
        <div class="hello2">안녕하세요.4</div>
        <div class="hello1 text_bold">안녕하세요.5</div>
        <div class="hello2 text_bold">안녕하세요.6</div>


    </body>
````

### 소속을 명확히 지정해준것이 우선순위가 높다
--------------------------------------------------------------------------------

- html 한 파일 안에 다 쓰지않고 Link 걸어줘서 사용하는경우가 많다.

## dispaly:block , display:inline
- dispaly:block : 어떤 영역을 고정으로 지정
- display:inline : 유동적인 콘텐츠에 유동적으로 영역을 설정

## margin , padding
- margin : 해당 오브젝트의 바깥 여백
- padding : 해당 오브젝트의 안쪽 여백

## width, height
- width : 가로너비
- height : 세로너비

## overflow
- 자식 elment가 부모 element 영역을 넘어가지 않도록 설정

## absolute
- element와 관계없이 해당 영역에서 원하는대로 자유롭게 위치를 잡아줌

## relative
- 관계 있게 작용...

## fixed
- 사용자가 스크롤을 움직여도 고정적으로 element를 fix시키고 싶을때 사용
- absolute와 다르게 fixed는 relative에 따라 기준점이 바뀌는 것이 아닌, 무조건 화면을 기준으로 위치를 잡는다는 것을 주의 해야함

## z-index
- z-index : 1,2,3 이런식으로 우선순위를 지정해서 element를 나타냄

## border, border-radius, box-sizing

### border
- 테두리를 주기 위해서는 border 속성을 이용
- 속성값으로는 총 세 가지를 한 번에 입력해야 함 (테두리 두께, 모양, 색상)
- 두께는 보통 px 단위
- 모양에는 solid, dotted 정도가 쓰임 solid : 기본선, dotted : 점선
- 몇가지 더 있지만 자세한건 ***W3school***에서 직접 보는 것 권장

### border-radius
- 버튼 같이 모서리의 굴곡을 만들기 위해 사용
- 값을 보통 50%라고 입력하면 쉽게 원 모양 만듬

### box-sizing
-padding이나 border가 기본 사이즈를 유지함

# p.60 Background 부터 하기
