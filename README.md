# bugyeong-next-app

부경사업단 업무앱 고도화 개발용 프로젝트입니다.

## 파일 구조
- `index.html` : 앱 런처
- `fc.html` : 가동관리(FC이미지제공)
- `manager.html` : 가동관리(지점/매니저 실적)
- `agency.html` : 대리점 실적
- `netlify.toml` : Netlify 배포 설정

## 운영 방식
GitHub에 파일을 업데이트하면 Netlify가 자동 배포합니다.


## PWA V1 추가
- `manifest.webmanifest` : 홈화면 설치 정보
- `service-worker.js` : 기본 캐시 및 오프라인 보조
- `icon-192.png`, `icon-512.png` : 앱 아이콘
- `index.html` : PWA 메타 및 서비스워커 등록 스크립트 추가

## GitHub 업로드 방법
압축을 풀고 모든 파일을 GitHub 저장소 루트에 업로드한 뒤 Commit 하면 Netlify가 자동 배포합니다.


## Supabase Ready V1 추가
- `admin.html` : Supabase URL/Anon Key 설정, 테이블 생성 SQL, 엑셀 미리보기 및 업로드
- `index.html` : 관리자 설정 메뉴 추가
- `service-worker.js` : 관리자 페이지 캐시 항목 추가

### 다음 작업
1. Supabase에서 새 프로젝트 생성
2. SQL Editor에 `admin.html`의 테이블 생성 SQL 실행
3. 관리자 설정 화면에서 Supabase URL / anon public key 입력
4. 엑셀 업로드 테스트
