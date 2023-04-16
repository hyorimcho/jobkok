# JOBKOK 📌
🥇 패스트캠퍼스 메가바이트 스쿨 3기 파이널 프로젝트 최우수상 수상 <br />

<img width="1021" alt="%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA_2023-04-10_%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE_5 00 07" src="https://user-images.githubusercontent.com/83855636/232267130-727049c5-eb9b-4ae0-9f58-faf61f86e3bf.png"><br />

> 지원자 모집부터 채용까지의 과정을 간편화하여 1인 기업 사장님들의 인사 업무 부담을 줄이고 원하는 인재와 자동으로 매칭 시켜주는 서비스입니다.

### 개발 기간
2023.03.03 ~ 2023.04.10

## 구현 기능

- 공통 레이아웃
  - navbar 구현
- 인재 상세 페이지
  - 인재 찜하기, 취소하기, 탈락 처리
    - 새로고침시에도 정보가 날아가지 않고 다른 페이지에서 나타나는 인재 정보에도 같은 정보가 표시됩니다.
    - 탈락 처리가 된 인재는 탈락 인재 보관함으로 이동합니다.
  - 타임라인
    - 서류 검토, 면접일 지정, 채용 확정을 기반으로 날짜가 입력되고 막대가 칠해집니다. 이전의 단계를 진행하지 않으면 다음 절차로 진행할 수 없습니다.
  - 면접 정보
    - 역시 react-query 의 useMutation 을 사용하여 정보를 업데이트 합니다. invalidateQueries를 사용하여 화면을 즉각적으로 업데이트 합니다.
  - 평가 노트
    - 기존에 평가가 되어있다면 그 평가를, 없다면 기본 메세지가 출력되어 평가를 할 수 있습니다.
- 알림센터
  - 필터링
    - react-query 의 select의 옵션을 사용해 채용 단계를 필터링하여 목록에 보여줍니다. 또한 useSearchParams 를 사용하여 새로고침시에도 정보가 유지됩니다.
  - 인재 선택 및 메세지 전송
    - 최대 4명의 인재에게 단체 메세지를 보낼 수 있습니다. 알림 단계에 따라 기본 메세지가 출력되며 react-hook-form 의 watch함수를 사용하여 글자수를 관리하며 1,000자 이상 입력할 수 없습니다. 메세지 입력 후 주의사항에 동의해야만 메세지 전송이 가능합니다.

## 기술 스택

- vite, react, typescript, redux-toolkit, tailwindcss, axios, react-hook-form, zod, react-router-dom, react-query

## 협업 방식

- 공통 소통 툴: 슬랙, 노션, 게더타운
- FE & UXUI: 피그마, 제플린
- FE & BE: 깃헙, 포스트맨


## 느낀 점
프로젝트 진행이 담긴 회고는 [블로그](https://velog.io/@hyorimm/%ED%8C%8C%EC%9D%B4%EB%84%90-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%EC%9D%B8%EC%82%AC-%EC%B1%84%EC%9A%A9-%EC%84%9C%EB%B9%84%EC%8A%A4-%EB%A7%8C%EB%93%A4%EA%B8%B0-%ED%9A%8C%EA%B3%A0)에 정리하였습니다.

## 팀원

<table border>
  <tbody>
    <tr>
       <td align="center" width="200px">
        <img width="100%" src="https://avatars.githubusercontent.com/u/83855636?v=4"  alt="유지석님"/><br />
        <br/>
        <a href="https://github.com/yujiseok">
          <img src="https://img.shields.io/badge/팀장 : 유지석-000?style=flat-round&logo=GitHub&logoColor=white"/>
        </a>
      </td>
      <td align="center" width="200px">
        <img width="100%" src='https://avatars.githubusercontent.com/u/90189513?v=4'  alt="이은영님"/><br />
        <br/>
        <a href="https://github.com/eun0leee">
          <img src="https://img.shields.io/badge/이은영-000?style=flat-round&logo=GitHub&logoColor=white"/>
        </a>
      </td>
      <td align="center" width="200px">
        <img width="100%" src="https://avatars.githubusercontent.com/u/113823957?v=4"  alt="이혜란님"/><br />
       <br/>
        <a href="https://github.com/hyerani">
          <img src="https://img.shields.io/badge/이혜란-000?style=flat-round&logo=GitHub&logoColor=white"/>
        </a>
      </td>
   <td align="center" width="200px">
        <img width="100%" src="https://avatars.githubusercontent.com/u/103406196?v=4"  alt="조효림님"/><br/>
       <br/>
        <a href="https://github.com/hyorimcho">
          <img src="https://img.shields.io/badge/조효림-000?style=flat-round&logo=GitHub&logoColor=white"/>
        </a>
      </td>
     </tr>
  </tbody>
</table>