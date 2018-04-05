# Practical Regular Expression

## 글로벌 플래그와 커서
- 커서 초기화 ([jsbin](http://jsbin.com/faxaleh/1/edit?js,console))
- 글로벌 플래그를 활용한 while 구문 ([jsbin](http://jsbin.com/fobiqub/edit?js,console))

## 그룹
- 그룹 상수 ([jsbin](http://jsbin.com/tuguqa/2/edit?js,console))
- 그룹 상수 + while ([jsbin](http://jsbin.com/viyuroq/2/edit?js,console))

## 멀티라인
- 멀티라인 플래그 활용 ([jsbin](http://jsbin.com/vaziwoc/1/edit?js,console))

## 한글
- \w는 한글을 포함하지 않음 ([regexp](https://regexr.com/3ncsc))
- \[\wㄱ-ㅎ가-힣] ([regexp](https://regexr.com/3ncsl)
- 유니코드를 포함한 모든 문자 (\[\s\S]) ([regexp](https://regexr.com/3ncsr))

## Positive/Nagative lookahead
- ?=, ?! ([regexp](https://regexr.com/3nct4)

## Greedy vs Non-Greedy
- 수량자 뒤 ? = non-greedy ([jsbin](http://jsbin.com/nuyuzub/1/edit?js,console))

## 조합
- 모두 정규식으로 해결하려고 하면 복잡해지고 디버깅하기 어려움 ([jsbin](http://jsbin.com/nodomuy/1/edit?js,console))

## 테스트 코드
- 복잡한 정규식은 테스트 코드를 남겨두면 디버깅하기 좋음 ([jsbin](http://jsbin.com/ruxokus/2/edit?js,console))
