Service Topic : 

직원 관리 시스템
직원들의 기본 인적 사항과 부서 정보를 등록, 조회, 수정, 삭제할 수 있는 웹 서비스입니다.

Data Fields :

사번 : 직원을 식별하는 6자리 고유 숫자

이름 : 직원의 성명

부서 : 직원이 소속된 부서

이메일 : 직원의 업무용 이메일 주소

연락처 : 직원의 휴대전화 번호

입사일 : 직원이 회사에 입사한 날짜

List Page : 

사번, 이름, 부서, 연락처, 상세보기로 이동할수있는 버튼

Validation : 

이름 입력 여부: 이름의 공백을 제거한 뒤 값이 비어있는지 검사 (name.trim() === "")

사번 길이: 사번이 정확히 6자리 숫자로 입력되었는지 검사 (empId.length !== 6)

Select 선택 여부: 부서 드롭다운 메뉴에서 기본값("부서 선택")인 채로 제출되었는지 검사 (dept === "")

이메일 형식: 정규표현식(/.+@.+\..+/)을 사용하여 '@'와 '.'이 포함된 올바른 이메일 구조인지 검증

RWD  : 

Desktop: Navigation 바의 메뉴를 우측 상단에 가로로 모두 펼쳐서 배치했습니다. 폼(Form) 페이지에서는 Grid를 적용해 한 줄에 2개의 입력창이 나란히 표시되도록 구성했습니다. Table 역시 모든 데이터가 한눈에 보이도록 가로로 넓게 배치했습니다.

Mobile: 모바일 환경(max-width: 768px 이하)에서는 Navigation 바가 우측 상단의 메뉴아이콘으로 자동으로 접힙니다. 폼 입력창은 한 줄에 1개씩 세로로 쌓이도록 배치되어 입력 편의성을 높였습니다. 좁은 화면에서 Table 전체가 깨지는 것을 막기 위해 테이블 영역 내부에서만 좌우로 밀어서 볼 수 있도록 가로 스크롤 기능을 활성화했습니다. 모바일에서는 누르기 쉽게 모든 버튼이 가로폭에 꽉 차도록(width: 100%) 적용했습니다.

Bootstrap : 

Layout/Grid: container, row, col-md-6, col-lg-8, g-3

Navigation: navbar, navbar-expand-lg, navbar-dark, bg-dark, navbar-toggler

Card & List: card, card-header, card-body, list-group, list-group-flush

Form: form-label, form-control, form-select

Table: table, table-hover, table-responsive, align-middle

Button & Badge: btn, btn-primary, btn-warning, btn-danger, btn-outline-secondary, badge, bg-info

Problem & Solution : 

문제: 이런 웹사이트를 만드는 경험이 처음이다 보니 화면배치나 조합들이 어떻게 해야하는지 어려움을 겪었고, 자바스크립트도 활용이 처음이다 보니 기능 구현에 어려움을 겪었다.

해결방법: AI를 이용해 일단 예시와 어떻게 배치해야하는지 보고 많이 보고 따라했다. 자바스크립트는 일단 공부를 해보면 작동이 안되면 AI에게 질문을 통해 해결하였다. 

Reflection : 
일단 문법의 코드를 다 외우는게 정답은 아닌걸 알게되었고, 그래도 기본적인 코드들을 알고있어야겠다고 깨달았고, 도움없이 최대한 혼자 만들어 보는게 진짜 많은 도움이 되겠다는 생각이 들었다. 그리고 이번 과제를 하며 부트스트림을 어떻게 활용하는지 더 알게되었다.
