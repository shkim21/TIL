내가 보려고 정리한 마크다운 문서 작성법
===============
앞으로 문서화를 잘 시키도록 하자!

문서 제목
=======

문서 부제목
--------
   
   

글머리
# 글머리1 (띄어쓰기 주의)  
## 글머리2
### 글머리3
#### 글머리4
##### 글머리5
###### 글머리 6

줄바꿈 : 스페이스바 3번!!   (or tab)
* 기호   
  * 줄바꿈   
    * 줄바꿈2   
      * ㅇㅇㅇ

BlockQuote
> 옆에 줄 있는거   
>   > 하나 더
>   >   > 또 하나 더

들여쓰기 : 탭 or 4개 공백(띄어쓰기 필요)   
    들여쓰기   
        들여쓰기2    

제일 중요한 코드블럭
<pre><code>
class SpringCamp(models.Model):
    name ~
    id ~

    </code></pre>

2번째 방법(요렇게 언어 지정가능!)
```python
class Camp(models.Model):
    name = CharField()

    def __str__(self):
        return self.name
```

수평선
***
여러가지 방법이 있음
*********

강조하기    
*기울이기*  
_요거도 기울이기_   
**굵은글씨**    
__굵은글씨(ver2)__  
~~취소선~~  
<u>밑줄이다잉</u>

링크삽입    
[GOOGLE](https://google.com)    
[CAFEGO](https://cafego.kr)     
[FIELDBY](https://fieldby.me)


