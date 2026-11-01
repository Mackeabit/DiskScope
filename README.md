# DiskScope

![DiskScope](DiskScope.png)

Windows용 읽기 전용 디스크 공간 탐색기입니다. 일반 권한으로 로컬 드라이브·폴더를 스캔하고, 큰 파일과 공간 분포를 목록·트리맵으로 살펴봅니다. 한국어 UI, 차콜 다크 테마, 포함된 Pretendard 폰트를 사용합니다.

**0.1.0 초기 미리보기.** Windows 10 Pro 22H2 x64 개발 PC에서 검증했습니다. **Windows 11과 개발 도구·런타임이 사전 설치되지 않은 깨끗한 PC에서는 아직 검증하지 않았습니다.** 이 미리보기는 다른 환경의 실행을 보장하지 않으며 실행 파일은 서명되지 않았습니다.

## 실행과 탐색

사용·재배포 전에 [BINARY-TERMS.txt](BINARY-TERMS.txt)와 안내된 전체 구성요소 약관을 읽고 동의해야 합니다. 동의하지 않으면 해당 구성요소를 사용·재배포하지 마세요.

[Windows x64 ZIP 다운로드](https://github.com/Mackeabit/DiskScope/releases/download/v0.1.0-preview.1/DiskScope-0.1.0-preview.1-win-x64.zip) · [SHA-256 확인](https://github.com/Mackeabit/DiskScope/releases/download/v0.1.0-preview.1/SHA256SUMS.txt) · [릴리스 안내](https://github.com/Mackeabit/DiskScope/releases/tag/v0.1.0-preview.1)

ZIP을 **폴더 전체로 압축 해제**하고 `DiskScope.App.exe`를 실행하세요. 함께 들어 있는 DLL·Assets·licenses를 유지해야 합니다. 관리자 권한이나 폰트 설치는 필요하지 않습니다.

1. 드라이브나 폴더를 선택하고 **스캔 시작**을 누릅니다. **취소**하면 확인한 부분 결과를 남깁니다.
2. 폴더를 더블클릭하거나 Enter로 들어가고 Alt+↑로 올라갑니다. 검색·확장자·큰 파일 목록으로 결과를 좁힙니다.
3. 목록·폴더 트리·트리맵에서 **우클릭 → 탐색기에서 위치 보기**로 실제 항목의 위치를 엽니다. 폴더에는 **폴더 열기** 메뉴도 있습니다.
4. **탐색기에서 열기** 버튼은 선택한 폴더의 내용 또는 파일의 위치를 엽니다. 선택이 없으면 현재 폴더를 엽니다.
5. 외부에서 삭제·이동한 내용은 **다시 스캔 / F5**로 반영합니다. 결과는 스캔하며 수집한 기록이고 실시간 파일 목록은 아닙니다.

## 숫자의 의미

- **논리 크기:** 파일 이름별 데이터 길이입니다. 같은 파일의 하드링크 이름이 여러 개면 이름마다 셉니다.
- **고유 할당:** 같은 볼륨·파일 ID가 사용하는 할당 공간을 한 번만 셉니다. 하드링크 별칭은 0 B로 표시될 수 있습니다. 삭제하면 확보되는 용량과 같지 않습니다.
- **미확인:** 접근 거부·제외·변경 등으로 확정하지 못한 부분입니다. 미확인 개수는 누락된 바이트 수가 아닙니다.

시스템 메타데이터·보호된 데이터·스캔 도중 변경 때문에 파일 합계가 드라이브 사용량과 다를 수 있습니다. 네트워크 스캔, 파일 삭제·정리, 관리자 전용 스캐너는 제공하지 않습니다. 재분석 지점과 클라우드/오프라인 표식은 기본적으로 따라가지 않습니다. 실제 클라우드 제공자, 화면 읽기 프로그램 및 다양한 DPI 환경의 검증은 남아 있습니다.

## 소스와 라이선스

이 저장소는 배포 안내용이며 **원본 소스 파일은 공개하지 않습니다**. 실행 ZIP에는 원본 C#/XAML/프로젝트/PDB 파일을 넣지 않습니다. 다만 .NET 실행 파일을 분석해 유사한 코드를 복원하는 것은 가능합니다.

DiskScope 원본 코드와 아이콘의 [MIT](LICENSE)는 유지합니다. MIT는 소스 제공을 요구하지 않으며, 소스 비공개가 MIT의 사용·복제·재배포 권리를 취소하지는 않습니다. 외부 구성요소는 [각자의 라이선스](THIRD-PARTY-NOTICES.md)를 따릅니다. Pretendard는 SIL OFL 1.1, Microsoft 서명 Win2D 바이너리는 별도 Microsoft 약관을 따릅니다. [전체 배포 조건](BINARY-TERMS.txt).

GitHub가 자동으로 만드는 **Source code (zip/tar.gz)**는 이 안내 저장소의 파일을 압축한 것입니다. 비공개 개발 저장소의 프로그램 소스가 들어가는 파일이 아닙니다. 실행하려면 `win-x64.zip` 자산을 받으세요.

DiskScope는 스캔 결과를 외부로 업로드하지 않습니다. 오류 로그에는 경로가 들어갈 수 있으므로 [보안·개인정보 안내](SECURITY.md)를 확인하세요.

[릴리스 정보와 알려진 한계](docs/RELEASE-NOTES.md)

## English

DiskScope is a read-only Windows disk-space explorer with a Korean, dark UI. Source files remain private; this repository contains distribution documentation only. The application ZIP contains compiled binaries, runtime components, fonts and notices. MIT remains applicable to the original work; bundled dependencies retain their own terms. Compiled .NET code can still be analyzed or decompiled. This unsigned early preview was tested on a Windows 10 development PC only. Windows 11 and clean-machine operation remain unverified.
