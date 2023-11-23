# 설치 패키지 
# 1) 메뉴 라이브러리 설치
npm i react-router-dom
npm i @types/react-router-dom

# 2) 벡엔드 연동 라이브러리 설치
npm i axios

# 3) pre css 컴파일러 : sass
npm i sass

# 4) Material Page component 업그레이드 
# 과거 v4 -> v5 변경 설치
npm i @mui/material @emotion/react @emotion/styled

# 4-1) 소스에서 임포트 사용법 : <Pagination />
import Pagination from '@mui/material/Pagination';

# 5) typescript jquery, jqueryui type 넣기
# 5-1) typescript jquery 사용
npm i --save-dev @types/jquery
npm i --save-dev @types/jqueryui

# 6) tiny-slider 설치
npm i tiny-slider@2.2.6
# 6-1) typescript tiny-slider
npm i --save @types/tiny-slider-react

# 사이드바 npm 설치
# 7-1) 스타일 컴포넌트 설치
npm install styled-components
npm install @types/styled-components --save-dev

# 7-2) 리액트 아이콘 npm
npm install react-icons --save

# TODO:8) 로그인 관련/공유라이브러리 리덕스-툴킷 설치
npm i react-redux @reduxjs/toolkit

# TODO:) 로그인 관련/폼 유효성 체크 라이브러리 설치
# TODO:8-2) formik
npm i formik

# TODO:8-3) 로그인 관련/yup
npm i yup
npm i @types/yup

<!-- 참고 -->
# * 외부 라이브러리 타입이 없을 경우 처리 : 타입 설정
# 1) tsconfig.json 파일 - compilerOptions 속성에 아래 추가 : 프로젝트시작위치/types - 이 위치에 타입을 인식하게 하는 경로 설정
"typeRoots": ["./types", "./node_modules/@types"], // 보통 types 폴더를 만들어 타입 정의
# 2) types/외부라이브러리명/index.d.ts 파일 생성 후 아래 추가
declare module '외부라이브러리명';