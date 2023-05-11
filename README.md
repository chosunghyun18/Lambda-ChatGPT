# Lambda-ChatGPT

AWS Lambda with OpenAI Library - ChatGPT

### 준비
- open ai api key 필요

- [여기](https://platform.openai.com/account/api-keys) 에서 가입 후 생성을 한다.

- lambda_function.py 생성 : 이름 일치 필수

### OpenAI Library 가 필요하여 pip 로 install 하기 위해 zip 으로 업로드 하여 Lambda Function 생성.
- 현제 파일 위치에 openai 라이브러리 압축 
- pip3 install openai -t .

- zip 파일로 압축 aws 람다 에서 업로드 
- zip -r aws-lambda-test.zip .

### 구성

일반구성 > 편집 > 제한시간을 적당히 늘려줌. (60초)

함수 URL > 생성

### 실행

함수 url 에 파라메터로 쿼리 날리기

https://api_lambda_key.ap-northeast-2.on.aws/?prompt=hellow~
