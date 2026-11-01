# v0.1.0-preview.1 — 초기 미리보기

2026-11-01 포터블 구성 갱신: ZIP 최상위에는 `DiskScope.App.exe`와 `app` 폴더만 있습니다. 전체를 압축 해제하고 최상위 EXE를 실행하세요. DLL·런타임·README·약관은 `app` 안에 함께 유지해야 합니다. 일반 권한 스캔과 용량·하드링크 계산, Windows App SDK 2.5.1은 유지했습니다.

소스는 비공개로 유지하며 공개 저장소에는 안내 문서와 라이선스만 제공합니다. 이 릴리스는 **Pre-release**입니다. **Windows 10 Pro 22H2 개발 PC에서만 검증한 미서명 초기 미리보기이며 Windows 11·깨끗한 PC는 미검증입니다.** 다른 환경의 실행을 보장하지 않습니다.

## DiskScope

일반 권한으로 로컬 드라이브·폴더의 저장 공간을 살펴보는 Windows용 읽기 전용 탐색기입니다.

- 파일 이름별 논리 크기와 하드링크 중복을 제외한 고유 할당을 구분합니다.
- 폴더 트리, 가상화 목록, 트리맵, 검색·필터, 탐색기 위치 열기를 제공합니다.
- 스캔 중 탐색과 취소를 지원하며 접근할 수 없는 항목은 미확인으로 남깁니다.
- 목록·폴더 트리·트리맵 우클릭에서 탐색기 위치 보기를 제공합니다. 폴더는 내용 열기와 상위 위치에서 선택하기를 구분합니다.
- 수집 시각과 재스캔 안내를 표시합니다. 외부 삭제·이동은 다시 스캔 또는 F5 후 반영하며, 사라진 경로 열기는 안내로 처리합니다.
- 차콜 다크 테마와 포함된 Pretendard를 사용합니다. 별도 폰트 설치가 필요하지 않습니다.
- Windows App SDK **2.5.1**, Win2D **1.4.0**을 고정했습니다.

자체 Windows 10 개발 PC의 같은 C: 재스캔 비교에서 메모리 최고치를 2.139 GiB에서 1.165 GiB로 줄였습니다. 파일시스템은 실행 중 변경되는 환경이며 모든 PC의 성능을 보장하는 수치는 아닙니다. 이번 탐색기 연동 변경에서 C: 전체 성능 측정을 다시 수행한 것은 아닙니다.

## 다운로드 전 약관 안내

DiskScope 원본 코드와 아이콘은 [MIT](../LICENSE)입니다. 실행 ZIP의 Win2D·Windows App SDK 등 Microsoft 구성요소에는 별도 약관이 적용됩니다. **사용·재배포 전에 [BINARY-TERMS.txt](../BINARY-TERMS.txt)와 링크된 전체 약관을 읽고 동의해야 하며, 동의하지 않으면 해당 구성요소를 사용·재배포하지 마세요.** 재배포 시 이 안내와 모든 고지·약관을 유지해야 합니다. [Win2D 약관 원문과 확인 근거](../licenses/SUPPLEMENTAL.md).

Before using or redistributing the bundled Microsoft components, read and agree to BINARY-TERMS.txt and the full component terms linked there. Do not use or redistribute those components if you do not agree. DiskScope's original code remains MIT licensed; third-party components are not relicensed under MIT.

## 배포 파일

| 파일 | 용도 / 현재 상태 |
| --- | --- |
| [DiskScope-0.1.0-preview.1-win-x64.zip](https://github.com/Mackeabit/DiskScope/releases/download/v0.1.0-preview.1/DiskScope-0.1.0-preview.1-win-x64.zip) | 폴더 전체를 풀고 `DiskScope.App.exe` 실행. 위 검증 범위의 초기 미리보기. |
| [SHA256SUMS.txt](https://github.com/Mackeabit/DiskScope/releases/download/v0.1.0-preview.1/SHA256SUMS.txt) | 위 실행 ZIP의 SHA-256. |

원본 소스 ZIP은 배포하지 않습니다. GitHub 자동 생성 Source code 압축 파일은 안내 저장소의 문서만 포함하며 프로그램 소스를 제공하지 않습니다. 실행 ZIP에도 원본 소스·프로젝트·PDB는 없지만 .NET DLL을 분석해 유사 코드를 복원하는 것은 가능합니다.

## 알려진 한계

- 현재 실제 검증은 Windows 10 Pro 22H2 x64 개발 PC입니다. Windows 11·깨끗한 PC 실행 검증은 아직 완료하지 않았습니다.
- 실행 파일은 서명되지 않았습니다. 안정판으로 표시하지 않습니다.
- UI는 한국어·다크 전용입니다. 화면 읽기 프로그램, 다중 모니터 DPI, 실제 클라우드 제공자의 다운로드 방지는 추가 검증이 필요합니다.
- 탐색기 연동과 실제 WinUI 메뉴 표시의 내부 통합 검사 13개를 통과했습니다. 이 개발 PC의 자동 입력 도구 오류로 실제 우클릭·Shift+F10 입력 검증은 남아 있습니다.
- UNC·네트워크 스캔, 관리자 전용 고속 스캔, 파일 삭제·정리는 제공하지 않습니다.
- 고유 할당은 삭제하면 확보되는 공간이 아닙니다. 접근 거부·재분석 지점·실시간 변경 때문에 합계가 드라이브 사용량과 다를 수 있습니다.

[사용 안내](../README.md) · [보안 제보](../SECURITY.md)
