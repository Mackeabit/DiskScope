# v0.1.0-preview.1

Windows용 읽기 전용 디스크 공간 탐색기 **DiskScope의 첫 미리보기**입니다.

## 주요 기능

- 드라이브·폴더 스캔, 진행 상황 표시와 취소
- 폴더 탐색·파일 목록·트리맵, 검색과 확장자 필터
- 논리 크기와 하드링크 중복을 제외한 고유 할당 표시
- 탐색기에서 위치 열기, **다시 스캔 / F5**로 결과 갱신
- 한국어 UI와 다크 테마, 포함된 Pretendard 폰트

## 다운로드와 실행

[Windows x64 ZIP 다운로드](https://github.com/Mackeabit/DiskScope/releases/download/v0.1.0-preview.1/DiskScope-0.1.0-preview.1-win-x64.zip) · [SHA-256](https://github.com/Mackeabit/DiskScope/releases/download/v0.1.0-preview.1/SHA256SUMS.txt)

ZIP 전체를 압축 해제하고 최상위 **`DiskScope.App.exe`**를 실행하세요. 함께 있는 **`app` 폴더를 유지**해야 합니다. 관리자 권한이나 별도 런타임·폰트 설치는 필요하지 않습니다.

## 참고사항

- Windows 10 22H2 x64에서 확인했습니다. Windows 11과 개발 도구·런타임이 없는 PC, 화면 읽기 프로그램·다중 모니터 DPI·클라우드 환경은 추가 검증이 필요합니다.
- 미서명 미리보기로 Windows 보안 경고가 표시될 수 있습니다.
- 외부에서 삭제·이동한 파일은 재스캔 후 반영됩니다. 고유 할당은 삭제 시 확보되는 공간과 다르며 접근 거부·제외·변경으로 합계가 드라이브 사용량과 다를 수 있습니다.
- 파일 삭제·정리, 네트워크 스캔, 관리자 전용 스캔은 제공하지 않습니다.

## 라이선스

원본 코드와 아이콘은 [MIT](../LICENSE)이며 포함된 외부 구성요소에는 [각자의 라이선스](../THIRD-PARTY-NOTICES.md)가 적용됩니다.

**사용·재배포 전에 [배포 약관](../BINARY-TERMS.txt)과 연결된 전체 구성요소 약관을 읽고 동의해 주세요. 동의하지 않으면 해당 구성요소를 사용·재배포하지 마세요.** 재배포 시 모든 약관과 저작권 고지를 유지해야 합니다.

[사용 안내](../README.md) · [보안·개인정보 안내](../SECURITY.md)
