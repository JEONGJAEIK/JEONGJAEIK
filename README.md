<div align="center">

![header](https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,100:16213e&height=230&section=header&text=Jaeik%20Jeong&fontAlign=50&fontAlignY=35&fontSize=50&fontColor=ffffff&desc=Backend%20Developer&descAlignY=55&descAlign=50&animation=fadeIn)
<br>

### 안녕하세요, 백엔드 개발자 정재익입니다

Java, Kotlin과 Spring으로 서버를 만들어 왔고,<br>
지금은 AI 에이전트 플랫폼의 인증과 외부 서비스 연동 권한 같은 서버 기반을 맡고 있습니다.

<br>

[![Blog](https://img.shields.io/badge/Tech%20Blog-jaeiktech.tistory.com-FF5722?style=for-the-badge&logo=tistory&logoColor=white)](https://jaeiktech.tistory.com)
[![Gmail](https://img.shields.io/badge/Gmail-wodlr1207@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:wodlr1207@gmail.com)

---
<br>

### 오픈소스 기여

| 프로젝트 | 내용 | 링크 |
|:---:|:---|:---:|
| **Hibernate ORM**<br><sub>머지</sub> | 비동기 스레드가 세션을 공유할 때 커넥션 해제 중 예외가 나면 물리 커넥션이 풀로 돌아가지 않던 누수 수정 | [PR](https://github.com/hibernate/hibernate-orm/pull/11468) [Blog](https://jaeiktech.tistory.com/76) |
| **Spring Data Redis**<br><sub>머지</sub> | 파이프라인을 닫을 때 타임아웃 같은 예외까지 다시 감싸 원인을 가리던 예외 처리 수정 | [PR](https://github.com/spring-projects/spring-data-redis/pull/3347) [Blog](https://jaeiktech.tistory.com/224) |
| **Prisma**<br><sub>리뷰 중</sub> | 외래키를 Prisma가 관리하는 설정에서 조건부 일괄 갱신이 UPDATE의 조건을 버리던 문제 수정 | [PR](https://github.com/prisma/prisma-engines/pull/5868) |

---
<br>

### 개인 프로젝트

<table>
  <tr>
    <td align="center" width="50%">
      <a href="https://github.com/BimilLog/BimilLog">
        <img src="https://github-readme-stats.vercel.app/api/pin/?username=BimilLog&repo=BimilLog&theme=tokyonight&hide_border=true" />
      </a>
      <br>
      <b>비밀로그</b> — 익명 롤링페이퍼 커뮤니티 서비스
      <br>
      <sub>Java · Spring Boot · JPA · QueryDSL · MySQL · Redis | 2025.04 ~ 2026.05 1인 개발</sub>
    </td>
    <td align="center" width="50%">
      <a href="https://github.com/JEONGJAEIK/MiniSpring">
        <img src="https://github-readme-stats.vercel.app/api/pin/?username=JEONGJAEIK&repo=MiniSpring&theme=tokyonight&hide_border=true" />
      </a>
      <br>
      <b>MiniSpring</b> — 순수 Java로 Spring의 핵심 동작을 직접 구현
      <br>
      <sub>컴포넌트 스캔 · 생성자 주입 · 트랜잭션 프록시 · 이벤트 리스너</sub>
    </td>
  </tr>
</table>

<br>

**비밀로그 성능 개선**

| 주제 | 요약 | 링크 |
|:---:|:---|:---:|
| **Redis 간헐 타임아웃 추적** | 커넥션 풀 없이 쓰던 파이프라인이 요청마다 TCP 연결을 맺고 끊어 Netty 이벤트 루프의 작업 큐가 밀린 것을 찾고, 커넥션 풀 설정과 캐시 구조 변경으로 게시판 조회 P99 11,802ms → 575ms | [Blog](https://jaeiktech.tistory.com/224) |
| **Redis 장애 대응 서킷 브레이커** | Redis 장애 때 로컬 캐시로 넘겨 장애 중 실시간 인기글 P99 6,034ms → 102ms, 정상 때 결과와의 유사도 20% → 93% | [Blog](https://jaeiktech.tistory.com/188) |
| **게시글 목록 조회 개선** | 커서 페이지네이션, 비정규화, Redis 캐시로 200ms 이내 응답 처리량 73.1 → 898.0 TPS | [Blog](https://jaeiktech.tistory.com/196) |
| **부하 테스트 오류 원인 추적** | Connection Refused를 OS 소켓 큐(파일 디스크립터, accept backlog)와 DB 커넥션 상한에서 찾아 조정하고, N+1 제거와 푸시 비동기화를 함께 적용해 최대 동시 사용자 416 → 1,000명, 오류율 50% → 0.1% | [Blog](https://jaeiktech.tistory.com/45) |

---
<br>

### Tech Stack

**Language**

![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

**Framework**

![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![JPA](https://img.shields.io/badge/JPA/Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white)
![QueryDSL](https://img.shields.io/badge/QueryDSL-0769AD?style=for-the-badge)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)

**Database & Cache**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?style=for-the-badge)

**Infrastructure & Monitoring**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge)
![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=for-the-badge&logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Sentry](https://img.shields.io/badge/Sentry-362D59?style=for-the-badge&logo=sentry&logoColor=white)
![JMeter](https://img.shields.io/badge/JMeter-D22128?style=for-the-badge&logo=apachejmeter&logoColor=white)
![Scouter](https://img.shields.io/badge/Scouter-1B1F23?style=for-the-badge&logo=opensourcehardware&logoColor=white)

---
<br>

### GitHub Stats & Algorithm

<a href="https://github.com/JEONGJAEIK"><img src="https://github-readme-stats.vercel.app/api?username=JEONGJAEIK&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="170" /></a>
<a href="https://github.com/JEONGJAEIK"><img src="https://github-readme-stats.vercel.app/api/top-langs/?username=JEONGJAEIK&layout=compact&theme=tokyonight&hide_border=true&hide=html,css" height="170" /></a>
<a href="https://solved.ac/wodlr1207"><img src="http://mazassumnida.wtf/api/v2/generate_badge?boj=wodlr1207" height="170" /></a>

---
<br>

### Education & Certificate

**컴퓨터공학 학사**(학점은행제) · 학점 4.5 / 4.5<br>
정보처리기사, 전자계산기기사, 전자계산기조직응용기사

<br>

![footer](https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,100:16213e&height=120&section=footer)

</div>
