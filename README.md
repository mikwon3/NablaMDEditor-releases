# ∇ NablaMDEditor

수식과 상호참조를 그대로 둔 채 한글(HWPX)·Word(DOCX)·PDF 로 내보내는 학술 Markdown 편집기입니다(macOS · Windows).

A Markdown editor for academic writing. It keeps equations and cross-references intact and exports to Hangul (HWPX), Word (DOCX) and PDF (macOS · Windows).

**이 저장소는 설치 파일만 배포합니다.** 앱 소스는 따로 관리합니다.

## 내려받기 · Download

**[최신 판 받기 · Latest release →](https://github.com/mikwon3/NablaMDEditor-releases/releases/latest)**

| 운영체제 | 파일 |
|---|---|
| macOS 12 이상 (Apple Silicon) | `NablaMDEditor-<판>.dmg` |
| Windows 10 이상 x64 (Windows 11 에서 확인) | `NablaMDEditor-<판>-amd64-installer.exe` |

각 릴리스에 SHA-256 체크섬을 적어 둡니다.

## 처음 열 때 경고가 뜹니다

설치 파일에 **개발자 서명이 없습니다.** 운영체제가 확인할 수 없는 앱이라고 경고합니다.

**macOS** — "확인할 수 없어 열 수 없습니다" 가 뜨면

1. **시스템 설정 › 개인정보 보호 및 보안** 에서 아래쪽의 **"그래도 열기"** 를 누릅니다.
2. 그래도 열리지 않으면 터미널에서 한 번 실행합니다.
   ```bash
   xattr -dr com.apple.quarantine /Applications/NablaMDEditor.app
   ```

**Windows** — "Windows의 PC 보호" 가 뜨면 **추가 정보 › 실행** 을 누릅니다.

## 핵심

- **수식과 상호참조** — `$…$`·`$$…$$` 를 KaTeX 로 그리고, 식·표·그림에 번호를 매겨 `[@eq:hooke]` 로 참조하면 **식 (1)** 로 나옵니다. 문법은 pandoc-crossref 표준입니다.
- **바로 보기 편집** — 커서가 있는 줄만 원문으로 두고 나머지는 그린 결과로 보여 줍니다.
- **한글(HWPX)·Word(DOCX) 내보내기** — 수식이 그림이 아니라 각 프로그램의 **수식 객체**로 나갑니다.
- **한글·Word 문서 읽기** — `.docx`·`.hwpx` 를 열어 고칩니다. 창에 끌어다 놓아도 열립니다.
- **문서 스타일** — 화면과 내보낸 결과가 같은 스타일 세트를 씁니다.
- **PDF 와 인쇄** — 용지·여백·방향을 정하고 그 자리에서 인쇄합니다.
- **표와 그림** — 표는 격자로 입력하고 엑셀에서 붙여넣습니다. 그림은 클립보드에서 바로 붙습니다.
- **AI 보조** — 문장 다듬기 · 표현 제안 · 개조식 · 요약하기 · 문체 바꾸기 · 수식 만들기 · 한↔영 번역. 결과는 원문과 나란히 보고 승인해야 들어갑니다.
- **오프라인 AI** — 앱에 담긴 llama.cpp 가 이 컴퓨터에서 GGUF 모델을 돌립니다. 인터넷도 API 키도 필요 없습니다.
- **원문은 Markdown 한 파일** — 앱 전용 형식이 없습니다.

## 이용 조건 · Terms

누구나 무료로 쓸 수 있습니다. 나눠 줄 때는 이 저장소 링크를 알려 주십시오.

Free for anyone to use. When sharing, please point people to this repository.

## 제3자 구성요소

설치 파일에는 Pandoc(GPL)·Python(PSF)·llama.cpp(MIT)·Pretendard·D2Coding(SIL OFL) 등이 함께 들어 있습니다.
각 라이선스와 소스 위치는 [NOTICE.md](NOTICE.md) 와 [licenses/](licenses/) 에 있습니다.

© 2026 경상국립대학교
