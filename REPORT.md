# A1 리포트

- 이름: 유진영
- 학번: 2023202052
- GitHub ID: jinyoung-yoo

## 어디를 둘러봤는지

Mad science, Hardware, Image, Text, Number, Math, Parsing 등의 카테고리를 둘러봄. 

터미널 검색어: npm search "qrcode"
경로: https://npm.im/qrcode

터미널 검색어: npm search "splice string"
경로: https://npm.im/splice-string

터미널 검색어: npm search "x-ray"
경로: https://npm.im/x-ray

---

## 선정한 패키지

### 1. qrcode

**선정 이유:**
텍스트나 URL을 스마트폰 카메라로 바로 스캔할 수 있는 QR 코드로 변환해 준다는 점이 실용적이고 신기해서 고르게 됨.

**이것으로 무엇을 할 수 있을지:**
터미널이나 웹 서비스에서 특정 웹사이트 주소나 Wi-Fi 접속 정보를 담은 QR 코드를 생성함. 이를 통해 정보를 제공할 때 QR 코드를 활용할 수 있음.

**확인 결과:**

```
$ npm view qrcode version time.modified license dependencies
version = '1.5.4'
time.modified = '2025-11-13T00:56:56.222Z'
license = 'MIT'
dependencies = { pngjs: '^5.0.0', yargs: '^15.3.1', dijkstrajs: '^1.0.1' }

$ npm view qrcode deprecated

```

**출력을 보고 알게 된 것:**
time.modified 값은 메타데이터 변경만으로도 갱신될 수 있어 정확한 최종 배포일로 단정하기는 어렵지만, 적어도 최근까지는 안전한 'MIT' 라이선스로 관리되고 있음을 알게 됨. 그리고 deprecated 출력이 없는 것으로 보아 현재도 활발히 유지보수되고 있는 패키지임을 알 수 있었음.

---

### 2. splice-string

**선정 이유:**
자바스크립트 기본 배열 메서드처럼 문자열의 특정 위치를 잘라내고 다른 문자를 쉽게 끼워 넣을 수 있는 기능이 직관적이라 선택함.

**이것으로 무엇을 할 수 있을지:**
예시로 사용자 입력 폼에서 전화번호의 특정 자리에 하이픈(-)을 처리할 때 문자열을 깔끔하게 수정하는 용도로 쓸 수 있음.

**확인 결과:**

```
$ npm view splice-string version time.modified license dependencies
version = '3.0.0'
time.modified = '2022-06-26T22:56:14.885Z'
license = 'MIT'
dependencies = { 'lodash.toarray': '^4.4.0' }

$ npm view splice-string deprecated

```

**출력을 보고 알게 된 것:**
마찬가지로 time.modified 값은 메타데이터 변경만으로도 갱신될 수 있어 정확한 최종 배포일로 단정하기는 어렵지만, 소형 패키지여서 최근 업데이트 빈도는 낮다는 것을 알게 됨. 하지만 라이선스가 'MIT'로 명확하고 deprecated 출력이 없어 안정적으로 사용할 수 있는 패키지임을 알 수 있었음.

---

### 3. x-ray

**선정 이유:**
인터넷 정보를 수집할 때 복잡한 설정 없이 간결하게 데이터를 긁어올 수 있는 웹 스크레퍼라는 설명이 흥미로워 고르게 됨.

**이것으로 무엇을 할 수 있을지:**
특정 사이트나 쇼핑몰 페이지에서 원하는 상품 가격이나 내용 등의 데이터를 간편하게 추출하여 데이터 수집 프로그램을 만들 수 있음.

**확인 결과:**

```
$ npm view x-ray version time.modified license dependencies
version = '2.3.4'
time.modified = '2022-06-29T04:38:46.066Z'
license = 'MIT'
dependencies = {
  batch: '~0.6.0',
  bluebird: '^3.4.7',
  chalk: '~2.4.0',
  cheerio: '~0.22.0',
  debug: '~4.1.0',
  enstore: '~1.0.1',
  'is-url': '~1.2.0',
  isobject: '~4.0.0',
  'object-assign': '~4.1.0',
  'stream-to-string': '^1.1.0',
  'x-ray-crawler': '~2.0.1',
  'x-ray-parse': '~1.0.1'npm install splice-string
}

$ npm view x-ray deprecated

```

**출력을 보고 알게 된 것:**
dependencies에 웹 파싱 핵심 라이브러리들이 잘 포함되어 있는 것을 확인함. 이를 통해 웹 스크레퍼 기능 구현에 최적화되어 있음을 알게 됨. 추가로 이전과 마찬가지로 time.modified 값은 메타데이터 변경만으로도 갱신될 수 있어 정확한 최종 배포일로 단정하기는 어렵지만, 2022년을 마지막으로 관리를 진행했으며, deprecated 출력이 없어 'MIT' 라이선스 하에 안정적으로 유지되고 있음을 알 수 있었음.

---

## 설치해본 패키지

```
$ npm install splice-string

$ node try.js
universe
```

---

## 막혔던 부분 (채점하지 않음)

에러 메시지든 헷갈렸던 부분이든 하나. 두 문장이면 됩니다. 없었으면 없었다고 적습니다.

```
없음.
```

---

## AI 사용

사용했다면 프롬프트와, AI의 설명이 실제와 달랐던 부분을 적습니다.
사용하지 않았다면 "사용하지 않음"이라고만 적으면 됩니다.

사용하지 않음.

---

## 제출 전 확인

- [ ] 저장소 이름이 `oss2026-a1`, 공개 범위가 Public
- [ ] `git status` 결과가 `nothing to commit, working tree clean`
- [ ] `node_modules` 폴더를 지우고 `npm install` → `node try.js` 를 다시 해도 실행됨
- [ ] 마지막 커밋을 push함
