로그스트림에서 모니터링시 한글이 깨진다.

![](.paas_images/3c429d55.png)

직접적으로 관련있는 것은 아니지만, 이 [가이드 문서](https://github.com/glqdlt/glqdlt.github.io-private/blob/master/_stash/2022-05-15-AzureWebAppJava_CD%EA%B5%AC%EC%84%B1.md#:~:text=%EB%A1%9C%EA%B7%B8%EC%8A%A4%ED%8A%B8%EB%A6%BC%EC%97%90%EC%84%9C%20%EB%AA%A8%EB%8B%88%ED%84%B0%EB%A7%81%EC%8B%9C%20%ED%95%9C%EA%B8%80%EC%9D%B4,%EC%9D%B8%EC%BD%94%EB%94%A9%20%EC%85%8B%EC%9D%84%20%EC%A0%81%EC%9A%A9%ED%95%B4%EC%A3%BC%EC%97%88%EB%8B%A4)를 보면 기본 문자 인코딩셋이 UTF-8 이 아닌것으로 보인다. (MS 니깐 윈도우 기반인듯)

따라서 아래처럼 자바 런타임 환경변수로 UTF-8 인코딩 셋을 적용해주었다

![](.paas_images/e07899d4.png)