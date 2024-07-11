<!--
**bnbnac/bnbnac** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

<!--
## 능동적인 개발자 홍성진입니다

**Email**: bnbnac@naver.com


흘러가는 대로 살던 저는 교도관으로 2년 반 동안 근무하며 열정을 찾았습니다. 이를 바탕으로 능동적인 개발자가 되기 위해 도전하고 있습니다. '전략적 팀 전투'라는 게임 관련 사이트인 [tftad.com](https://tftad.com/) 개발을 진행하며 웹개발의 기본에 대해 알게 됐습니다. 또한 게시글 업로드 기능을 위해 필요한 라이브러리를 조사하여 보조서버를 개발한 경험이 있습니다. 목표를 설정하고 단계적으로 달성해 나가는 것을 좋아합니다.

&nbsp;
&nbsp;
&nbsp;

## 기술

Spring boot, JPA

&nbsp;
&nbsp;
&nbsp;

## 프로젝트

### (개인) tftad.com 백엔드([Github](https://github.com/bnbnac/tftad))

**배포: [tftad.com](https://tftad.com) (홈서버)**

온라인게임 Team-Fight-Tactics(전략적 팀 전투, 롤토체스) 요소 중 하나인 `증강체 선택` 관련 웹사이트입니다. 유튜브 크리에이터가 본인의 플레이 영상을 tftad.com로 게시 요청하면 JPA를 사용하여 DB에 게시글을 저장하고, [추출 서버](https://github.com/bnbnac/augment-extractor)에 `증강체 선택` 장면 추출을 요청합니다.

기술

- Spring boot, JPA

특징

- Rest API 서버입니다.
- [OAuth를 이용해 Member에 Channel을 등록합니다.(Blog)](https://velog.io/@bnbnac/Google-OAuth%EB%A5%BC-%EC%9D%B4%EC%9A%A9%ED%95%98%EC%97%AC-%EC%9C%A0%ED%8A%9C%EB%B8%8C-%EC%B1%84%EB%84%90-%EB%93%B1%EB%A1%9D%ED%95%98%EA%B8%B0)
- 게시글은 곧 `증강체 선택` 콘텐츠입니다. 따라서 게시글 작성 시 유튜브 영상 주소를 첨부해야 하고, 그 전에 계정에 유튜브 채널을 등록해야 합니다. [비즈니스 구조도 보러가기](https://drive.google.com/file/d/10TQxXs86JlJcG9l03tJL9e7Imm5rXgAT/view?usp=drive_link)([다크모드로 보러가기](https://drive.google.com/file/d/1l3K2C0_6eXKJbfeXUAosnXFnEVY0pFtR/view?usp=drive_link))
- 게시글 작성 시 관련 정보를 [추출 서버](https://github.com/bnbnac/augment-extractor)로 전송합니다. 이후 [추출 서버](https://github.com/bnbnac/augment-extractor)로부터 완료 정보를 받습니다.

&nbsp;
&nbsp;
&nbsp;
### (개인) tftad.com 보조서버([Github](https://github.com/bnbnac/augment-extractor))

클라이언트가 영상 게시를 요청하면 [tftad 서버](https://github.com/bnbnac/tftad)는 Augment-Extractor로 관련 정보를 전송합니다. Augment-Extractor는 비디오를 다운받고, 분석하고, 필요한 장면을 추출하여 storage 서버에 저장합니다.

기술

- Flask, [OpenCV](https://github.com/opencv/opencv), [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)

특징

- [OpenCV와 Tesseract OCR을 이용하여 증강체 선택장면을 추출합니다.(Blog)](https://velog.io/@bnbnac/OpenCV%EC%99%80-Tesseract-OCR%EC%9D%84-%EC%9D%B4%EC%9A%A9%ED%95%98%EC%97%AC-%EC%A6%9D%EA%B0%95%EC%B2%B4-%EC%84%A0%ED%83%9D%EC%9E%A5%EB%A9%B4-%EC%B6%94%EC%B6%9C%ED%95%98%EA%B8%B0)
- 추출 장면들을 잘라서 storage 서버에 전송합니다. 그리고 [tftad 서버](https://github.com/bnbnac/tftad)로 완료 request를 전송합니다.
- [worker queue를 유지하여 현재 작업 정보 반환하는 기능을 갖습니다.(Blog)](https://velog.io/@bnbnac/worker-queue%EB%A5%BC-%EC%9C%A0%EC%A7%80%ED%95%98%EC%97%AC-%ED%98%84%EC%9E%AC-%EC%9E%91%EC%97%85-%EC%A0%95%EB%B3%B4-%EB%B0%98%ED%99%98%ED%95%98%EA%B8%B0)
- [멀티스레딩을 활용하여 작업속도를 향상시킵니다.(Blog)](https://velog.io/@bnbnac/%EB%A9%80%ED%8B%B0%EC%8A%A4%EB%A0%88%EB%94%A9)

-->

