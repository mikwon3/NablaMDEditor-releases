# 제3자 구성요소 · Third-party components

NablaMDEditor 설치 파일에 함께 들어 있는 남의 것들과 그 라이선스입니다.

## 설치 파일에 함께 담기는 프로그램

| 구성요소 | 판 | 라이선스 | 전문 | 소스 |
|---|---|---|---|---|
| Pandoc | 3.10.2 | GNU GPL v2 이상 (© 2006–2025 John MacFarlane) | [licenses/pandoc-COPYING.md](licenses/pandoc-COPYING.md) | [jgm/pandoc 3.10.2](https://github.com/jgm/pandoc/tree/3.10.2) · [tar.gz](https://github.com/jgm/pandoc/archive/refs/tags/3.10.2.tar.gz) |
| Python | 3.12.14 | PSF License | [licenses/python-LICENSE.txt](licenses/python-LICENSE.txt) | [python/cpython v3.12.14](https://github.com/python/cpython/tree/v3.12.14) |
| llama.cpp (`llama-server`, `ggml`) | b10793 | MIT (© 2023–2026 The ggml authors) | [licenses/llama.cpp-LICENSE.txt](licenses/llama.cpp-LICENSE.txt) | [ggml-org/llama.cpp b10793](https://github.com/ggml-org/llama.cpp/tree/b10793) |

- **Pandoc** 은 upstream 이 배포한 실행 파일을 **고치지 않고** 그대로 담습니다. 대응하는 소스는 위 링크의 3.10.2 태그입니다.
- **Python** 은 [astral-sh/python-build-standalone](https://github.com/astral-sh/python-build-standalone) 빌드를 씁니다. 그 안에 든 라이브러리(OpenSSL·SQLite·zlib·libffi 등)의 라이선스는 그 프로젝트에 정리되어 있습니다.
- **llama.cpp** 모델(GGUF)은 담지 않습니다. 사용자가 받거나 고릅니다.

## 앱에 들어 있는 글꼴

| 글꼴 | 판 | 라이선스 | 전문 |
|---|---|---|---|
| Pretendard | 1.309 (Kil Hyung-jin) | SIL OFL 1.1 | [licenses/Pretendard-OFL.txt](licenses/Pretendard-OFL.txt) |
| D2Coding | 1.3.3 (NAVER Corporation) | SIL OFL 1.1 | [licenses/D2Coding-OFL.txt](licenses/D2Coding-OFL.txt) |

## 앱에 컴파일되어 들어간 라이브러리

Wails, React, CodeMirror, KaTeX, markdown-it 등을 씁니다. 각 라이선스는 그 프로젝트에 있습니다.

## NablaMDEditor 저작자가 만든 부분

한글(HWPX) 내보내기 변환기와 그 서식 파일(`default_skeleton.hwpx`)은 NablaMDEditor 의 저작자가
Claude 와 함께 만든 것으로, 앱과 같은 저작자의 것입니다.
