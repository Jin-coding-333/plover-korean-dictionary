# 📘 Plover Korean Dictionary

한국어 속기(스테노) 입력을 위해 기능을 제공하는 [Plover](https://github.com/openstenoproject/plover) 앱의 플러그인인 [plover_korean](https://github.com/nsmarkop/plover_korean?utm_source=chatgpt.com)의 기본적인 키 동작이 맵핑 돼 있는 사전(dictionary) 모음집입니다.

사전을 사용하면 Glove80 같은 키보드에서 초성+중성+종성 조합 규칙을 기반으로 한글을 빠르고 정확하게 입력할 수 있습니다.

[plover_korean](https://github.com/nsmarkop/plover_korean?utm_source=chatgpt.com)에 사전이 올라와 있지만 정확히 인식되지 않는 버그가 있어 `json` 파일(**Plover**에서 제대로 인식하는 버전)으로 올렸습니다.

## ✨ 주요 기능

✅ 한글 자모 조합 지원: 초성, 중성, 종성 전부 스테노 stroke로 변환

✅ 사전 구성

- hangul_steno.json: 기본 자모/단어 매핑

- combos.json: 복합어·복합음절 단축 조합

- orthography.json: 맞춤법·결합 규칙 정의

✅ 호환성: Plover 4.0+ / plover_korean 플러그인

✅ 확장 가능: 사용자 정의 단어·단축어를 쉽게 추가 가능

## 📂 레포지토리 구조
```pgsql
plover-korean-dictionary/
├── dictionaries/
│   ├── hangul_steno.json   # 기본 한글 자모 사전
│   ├── combos.json         # 복합어/단축 조합
│   └── examples.json       # (선택) 예제용 확장 사전
├── orthography.json        # 초성+중성+종성 조합 규칙
└── README.md
```

## 🚀 설치 및 사용법

Plover 설치 후 plover_korean
 플러그인 활성화

이 레포를 클론하거나 ZIP 다운로드:
```bash
git clone https://github.com/Jin-coding-333/plover-korean-dictionary.git
```

dictionaries/*.json 파일을 Plover 설정 경로에 복사

macOS: `~/Library/Application Support/plover/dictionaries/`

Windows: `%APPDATA%\plover\dictionaries\`

Linux: `~/.local/share/plover/dictionaries/`

Plover → Configure → Dictionaries → +Add 에서 JSON 파일 추가

System을 Korean (CAS) 로 변경 후 Enable

## 🖥️ 예시

입력: `ㅅ + ㅏ`

출력: **사**

입력: `ㅎ + ㅏ + ㄴ + ㄱ`

출력: **한국**

## 📌 참고

[Plover 공식 문서](https://github.com/openstenoproject/plover/wiki)

[plover_korean 플러그인](https://github.com/nsmarkop/plover_korean?utm_source=chatgpt.com)
