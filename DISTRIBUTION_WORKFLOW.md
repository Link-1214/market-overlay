# Market Overlay 배포 정책

이 저장소는 일반 사용자 배포용입니다. 설치 파일, 사용자 가이드, 패치노트, 릴리즈 노트, 공개용 이미지와 해시 파일만 둡니다.

## 저장소 역할

- public distribution repo: 설치본과 사용자 문서 공개.
- private source repo: 소스 코드, 테스트, 빌드 스크립트, 내부 운영 문서 관리.

public repo의 GitHub `Source code(zip/tar.gz)` 자동 압축에는 실제 Python 앱 소스가 들어가지 않아야 합니다.

## 릴리즈 보관 정책

1. private source repo에서 설치본을 빌드하고 테스트합니다.
2. 최종 설치본과 공개 문서를 public repo의 `releases/vX.Y/`와 최신 루트 문서에 복사합니다.
3. 버전별 폴더에는 `SHA256SUMS.txt`를 함께 둡니다.
4. public repo에 `.py`, `.pyw`, `.ps1`, `.iss`, `tests/`, `tools/`, 내부 문서, 개인 데이터가 없는지 확인합니다.
5. GitHub Release에는 설치본과 SHA-256을 첨부합니다.

## 공개 문서 정책

- 최신 텍스트 가이드, 패치노트, 릴리즈 노트, 스크린샷 가이드는 루트 또는 `docs/`에 둡니다.
- 최신 스크린샷 가이드: `docs/USER_GUIDE_SCREENSHOT_V2_2.md`
- 현재 공개 이미지 폴더: `docs/images/user_guide_v2_0/`
- 스크린샷은 샘플 데이터 또는 완전히 비식별화된 데이터만 사용합니다.
- 오너 개인 장부, AppData 백업, 빌드 로그, 내부 운영 메모는 public repo에 두지 않습니다.

## 과거 버전

v1.8 이하 폴더는 로컬 릴리즈 아카이브에서 재구성한 보관본입니다. 다운로드와 변경 이력 확인용이며 전체 소스 히스토리로 보지 않습니다.
