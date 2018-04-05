# Practical Regular Expression

## 그룹


## 글로벌 플래그와 커서

- 글로벌 플래그를 설정하면 커서가 설정됨
- 글로벌 플래그를 활용한 while 구문 ([jsbin](http://jsbin.com/fobiqub/edit?js,console))
  ```js
  const str = 'foo bar foo baz';
  const rFoo = /foo/g;

  console.log('-[1]----------------');
  let fooCount = 0;
  while (rFoo.test(str)) {
    fooCount++;
  }
  console.log(fooCount);

  console.log('-[2]----------------');
  let i = 0;
  while (/foo/g.test(str)) { // Infinite loop
    if (i++ > 10) {
      break;
    }
  }
  console.log(i);
  ```

- 커서 초기화 ([jsbin](http://jsbin.com/faxaleh/1/edit?js,console))

  ```js
  const rFoo = /foo/g;

  const str = 'foo';
  const str2 = 'foobarbaz';

  console.log('-[1]----------------');
  console.log(rFoo.test(str), rFoo.lastIndex); //-> true
  console.log(rFoo.test(str), rFoo.lastIndex); //-> false

  console.log('-[2]----------------');
  console.log(rFoo.test(str), rFoo.lastIndex); //-> true
  console.log(rFoo.test(str2), rFoo.lastIndex); //-> false

  console.log('-[3]----------------');
  console.log(rFoo.test(str), rFoo.lastIndex); //-> true
  rFoo.lastIndex = 0; // 초기화
  console.log(rFoo.test(str2), rFoo.lastIndex); //-> true
  ```

## 멀티라인


## 워드블럭
- \b


## 한글
- \w는 한글이 아님
- [ㄱ-ㅎ가-힣]


## 모든 문자
- [\s\S]


## Greedy vs Non-Greedy
- 


## 조합
- 모두 정규식으로 해결하려고 하면 복잡해지고 디버깅하기 어려움


## 테스트 코드



