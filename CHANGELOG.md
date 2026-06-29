# Market Overlay Changelog

## v2.2

- 시장 데이터 provider 분리.
- v2.1 Yahoo 전일 종가 결측 보정 로직을 provider 경계와 회귀 테스트 안으로 정리.
- state `schema_version`과 legacy migration 도입.
- 진단 로그와 설정 탭 `로그 폴더 열기` 추가.
- 포트폴리오 비중/트리맵 시각화 영역 QSplitter 적용.
- offscreen 시각 회귀 스모크 테스트 추가.
- 내장 종목명 데이터 최신화.

## v2.1.1

- 미국, KRX, JPX 내장 종목명 데이터 확장과 검증 보강.

## v2.1

- GitHub 업데이트 확인 기능 추가.
- 트리맵 용어와 state 호환 이관.
- 시각화, 오버레이, worker, 앱 생명주기 코드 분리.

## v2.0

- 설치/제거 UX 보강.
- 공개/비공개 GitHub 운영 구조 정리.
- 스크린샷 기반 사용자 가이드 정리.
