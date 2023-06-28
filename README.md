- main : header




> topBar
>> primary-color 부여

>headerBox
>>flex로 column 형식 부여
>>div__memberSystem
>>>flex로 row 형식 부여하여 회원가입|로그인|고객센터 구현

>>headerBox__middle
>>>logo
>>>>flex로 row 형식 부여하여 로고와 마켓칼리 글자 형태 구현

>>>searchForm
>>>> 검색창 구현

>>>imoji
>>>>flex로 row 형식 부여하여 location, heart, shopping 배치

</br>
</br>

#### 1. 제목 등 보이지 않아도 되는 성질에 a11yHiddne class로 숨김처리 했습니다.
</br>

#### 2. 웹 접근성 향상을 위해 X , | 등 읽지 않아도 되는 표시자에는 aria-hidden 속성을 부여했습니다.
</br>

#### 3. 대부분의 코드에 부모-자식 간의 class연결성을 만들어두어 scss에서 편하게 구조화하고, 편하게 볼 수 있도록 구성하였습니다. (ex. searchForm(부모) - searchForm__group(자식))
</br>

#### 4. label과 legend, ul 등을 최대한 적재적소에 사용하여 더욱 코드를 symentic하게 구성하였습니다.


</br>
</br>

- main : nav

>category
>>자식요소인 categoryHover에 absolute주기 위해 relative 부여
</br>
>>Hamburger와 카테고리 부분 배치 위해 flex로 row 형식 부여
</br>
</br>
>>categoryHover
>>>flex형식으로 column주어 세로형식 배치
</br>
>>>justify : space-evenly 형식으로 균등배치
</br>
>>>기본 형식 visibility : hidden으로 숨김처리
</br>
</br>
>>>.category:hover > .categoryHover
>>>>category에 hover시 하위내역인 categoryHover에 변경사항 부여
</br>
>>>>visibility : visible 으로 보이게 처리
</br>
>>>>top : 40px 으로 위치 부여
</br>
</br>
>>>> 이후 각 카테고리 별 이미지 sprite로 부여

</br>
</br>

>navCenter
>> flex를 row형식으로 주어서 상단 nav바 배치
</br>
>> __new , __best , __hotdeal , __special
>>> 각 상자별 flex 위한 넓이 부여
</br>
>>>> hover
>>>>> hover시 글자 색깔 변화 및 및줄 부여

</br>
</br>

>morningDelivery
>>상자 배치 및 내부 글자 색깔 변경
</br>
>>상자 내부 flex형태 row 부여

</br>
</br>

#### 1. 카테고리 구성 중 다른 페이지와 class이름이 겹치는 상황이 발생하여, 다음에 프로젝트를 진행 시 평범한 class명 대신 unique하게 만들어야겠다고 생각했습니다.
</br>

#### 2. 다양한 이미지에 대체텍스트를 부여하여 접근성을 높혔습니다.
</br>

#### 3. 공통적으로 들어가는 부분을 mixin으로 대체하면 좋았을 것 같다고 생각됩니다. ex(너비, flex와 justify 등)



[google](google.com)

<img src="./src/images/favicon/favicon-192x192.webp" href="https://karly-css3.netlify.app/index.html">

[<img src="./src/images/favicon/favicon-192x192.webp"  width="10%" height="10%">](https://karly-css3.netlify.app/index.html)