<div align="center">

# jcode

[![Latest Release](https://badgen.net/github/release/1jehuang/jcode?icon=github)](https://github.com/1jehuang/jcode/releases)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](LICENSE)
[![Platforms](https://img.shields.io/badge/platforms-Linux%20%7C%20macOS%20%7C%20Windows-blue?style=flat-square)](https://github.com/1jehuang/jcode/releases)
[![Last Commit](https://badgen.net/github/last-commit/1jehuang/jcode/master?icon=github)](https://github.com/1jehuang/jcode/commits/master)
[![GitHub Stars](https://badgen.net/github/stars/1jehuang/jcode?icon=github)](https://github.com/1jehuang/jcode/stargazers)
[![Discord](https://img.shields.io/badge/Discord-Join%20Community-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.gg/nBe9vGyK9a)

가장 RAM 효율적인 하네스 <br>
가장 지능적인 하네스

<a href="https://trendshift.io/repositories/25042?utm_source=repository-badge&amp;utm_medium=badge&amp;utm_campaign=badge-repository-25042" target="_blank" rel="noopener noreferrer"><img src="https://trendshift.io/api/badge/repositories/25042" alt="1jehuang/jcode | Trendshift" width="250" height="55"></a>

<a href="https://github.com/1jehuang/jcode/releases/download/readme-assets/jcode-yc-launch.mp4">
  <img src="https://github.com/1jehuang/jcode/releases/download/readme-assets/jcode-yc-launch.webp" alt="jcode YC launch video" width="800">
</a>

<br>

[Website](https://jcode.sh) · [Docs](https://jcode.sh/docs) · [SDK](https://jcode.sh/sdk) · [Benchmarks](https://jcode.sh/bench) · [Features](#features) · [Install](#installation) · [Quick Start](#quick-start) · [Further Reading](#further-reading) · [Contributing](CONTRIBUTING.md)

</div>

---

<div align="center">

## 설치

</div>

```bash
# macOS & Linux
curl -fsSL https://jcode.sh/install | bash
```

```powershell
# Windows 11 (PowerShell 5.1+)
irm https://jcode.sh/install.ps1 | iex
```

Homebrew, 소스 빌드, 프로바이더 설정이 필요하거나 에이전트가 대신 설치해주길 원하시나요?
[상세 설치](#detailed-installation)로 이동하세요.

---


<div align="center">

## 성능 및 자원 효율성

</div>

jcode는 최대한 성능이 뛰어나고 자원 효율적으로 만들어졌습니다. 모든 지표는 뼛속까지 최적화되어 있으며, 이는 멀티 세션 워크플로우를 확장하는 데 중요합니다. 여기서는 RAM 사용량과 부팅 속도라는 몇 가지 지표를 샘플로 보여드립니다.

### RAM 비교

<div align="center">

<table>
  <tr>
    <td valign="top" align="center" width="50%">
      <strong>활성 세션 1개</strong>
      <table>
        <thead>
          <tr>
            <th>도구</th>
            <th>PSS</th>
            <th>비교</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><strong>jcode (로컬 임베딩 끔)</strong></td>
            <td align="right"><strong>27.8 MB</strong></td>
            <td align="right">기준</td>
          </tr>
          <tr>
            <td><strong>jcode</strong></td>
            <td align="right"><strong>167.1 MB</strong></td>
            <td align="right"><strong>RAM 6.0배</strong></td>
          </tr>
          <tr>
            <td><strong>pi</strong></td>
            <td align="right"><strong>144.4 MB</strong></td>
            <td align="right"><strong>RAM 5.2배</strong></td>
          </tr>
          <tr>
            <td><strong>Codex CLI</strong></td>
            <td align="right"><strong>140.0 MB</strong></td>
            <td align="right"><strong>RAM 5.0배</strong></td>
          </tr>
          <tr>
            <td><strong>OpenCode</strong></td>
            <td align="right"><strong>371.5 MB</strong></td>
            <td align="right"><strong>RAM 13.4배</strong></td>
          </tr>
          <tr>
            <td><strong>GitHub Copilot CLI</strong></td>
            <td align="right"><strong>333.3 MB</strong></td>
            <td align="right"><strong>RAM 12.0배</strong></td>
          </tr>
          <tr>
            <td><strong>Cursor Agent</strong></td>
            <td align="right"><strong>214.9 MB</strong></td>
            <td align="right"><strong>RAM 7.7배</strong></td>
          </tr>
          <tr>
            <td><strong>Claude Code</strong></td>
            <td align="right"><strong>386.6 MB</strong></td>
            <td align="right"><strong>RAM 13.9배</strong></td>
          </tr>
          <tr>
            <td><strong>Antigravity CLI</strong></td>
            <td align="right"><strong>243.7 MB</strong></td>
            <td align="right"><strong>RAM 8.8배</strong></td>
          </tr>
        </tbody>
      </table>
    </td>
    <td width="24"></td>
    <td valign="top" align="center" width="50%">
      <strong>활성 세션 10개</strong>
      <table>
        <thead>
          <tr>
            <th>도구</th>
            <th>PSS</th>
            <th>비교</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><strong>jcode (로컬 임베딩 끔)</strong></td>
            <td align="right"><strong>117.0 MB</strong></td>
            <td align="right">기준</td>
          </tr>
          <tr>
            <td><strong>jcode</strong></td>
            <td align="right"><strong>260.8 MB</strong></td>
            <td align="right"><strong>RAM 2.2배</strong></td>
          </tr>
          <tr>
            <td><strong>pi</strong></td>
            <td align="right"><strong>833.0 MB</strong></td>
            <td align="right"><strong>RAM 7.1배</strong></td>
          </tr>
          <tr>
            <td><strong>Codex CLI</strong></td>
            <td align="right"><strong>334.8 MB</strong></td>
            <td align="right"><strong>RAM 2.9배</strong></td>
          </tr>
          <tr>
            <td><strong>OpenCode</strong></td>
            <td align="right"><strong>3237.2 MB</strong></td>
            <td align="right"><strong>RAM 27.7배</strong></td>
          </tr>
          <tr>
            <td><strong>GitHub Copilot CLI</strong></td>
            <td align="right"><strong>1756.5 MB</strong></td>
            <td align="right"><strong>RAM 15.0배</strong></td>
          </tr>
          <tr>
            <td><strong>Cursor Agent</strong></td>
            <td align="right"><strong>1632.4 MB</strong></td>
            <td align="right"><strong>RAM 14.0배</strong></td>
          </tr>
          <tr>
            <td><strong>Claude Code</strong></td>
            <td align="right"><strong>2300.6 MB</strong></td>
            <td align="right"><strong>RAM 19.7배</strong></td>
          </tr>
          <tr>
            <td><strong>Antigravity CLI</strong></td>
            <td align="right"><strong>1021.2 MB</strong></td>
            <td align="right"><strong>RAM 8.7배</strong></td>
          </tr>
        </tbody>
      </table>
    </td>
  </tr>
</table>

</div>

### 첫 프레임까지 걸리는 시간

<div align="center">

| 도구 | 첫 프레임까지 시간 | 범위 | 비교 |
|---|---:|---:|---:|
| **jcode** | **14.0 ms** | 10.1–19.3 ms | 기준 |
| **Antigravity CLI** | **383.5 ms** | 363.1–415.4 ms | **27.4배 느림** |
| **pi** | **590.7 ms** | 369.6–934.8 ms | **42.2배 느림** |
| **Codex CLI** | **882.8 ms** | 742.3–1640.9 ms | **63.1배 느림** |
| **OpenCode** | **1035.9 ms** | 922.5–1104.4 ms | **74.0배 느림** |
| **GitHub Copilot CLI** | **1518.6 ms** | 1357.4–1826.8 ms | **108.5배 느림** |
| **Cursor Agent** | **1949.7 ms** | 1711.0–2104.8 ms | **139.3배 느림** |
| **Claude Code** | **3436.9 ms** | 2032.7–8927.2 ms | **245.5배 느림** |

</div>

이 Linux 머신에서 10회의 대화형 PTY 실행을 기준으로 측정했습니다.

### 첫 입력까지 걸리는 시간
(입력한 프로브 텍스트가 렌더링된 화면에 나타날 때까지의 시간. Antigravity는 로그인 화면이 프로브 에코를 억제하기 때문에 내부 입력 준비 로그 마커를 사용합니다.)
<div align="center">

| 도구 | 첫 입력까지 시간 | 범위 | 비교 |
|---|---:|---:|---:|
| **jcode** | **48.7 ms** | 30.3–62.7 ms | 기준 |
| **Antigravity CLI** | **383.7 ms** | 363.4–415.7 ms | **7.9배 느림** |
| **pi** | **596.4 ms** | 373.9–955.2 ms | **12.2배 느림** |
| **Codex CLI** | **905.8 ms** | 760.1–1675.7 ms | **18.6배 느림** |
| **OpenCode** | **1047.9 ms** | 931.1–1116.9 ms | **21.5배 느림** |
| **GitHub Copilot CLI** | **1583.4 ms** | 1422.8–1880.0 ms | **32.5배 느림** |
| **Cursor Agent** | **1978.7 ms** | 1727.3–2130.0 ms | **40.6배 느림** |
| **Claude Code** | **3512.8 ms** | 2137.4–9002.0 ms | **72.2배 느림** |

</div>

이 Linux 머신에서 10회의 대화형 PTY 실행을 기준으로 측정했습니다. Antigravity CLI는 이번 실행에서 인증되지 않은 상태였습니다. 로그인 화면은 정상적으로 렌더링되었고 내부적으로 `CLI ready for user input` 마커를 발생시켰지만, 입력한 프로브를 에코하지는 않았습니다.

### 추가 클라이언트 / 메모리 확장성

<div align="center">

| 도구 | 세션 추가당 PSS 증가량 | 비교 |
|---|---:|---:|
| **jcode (로컬 임베딩 끔)** | **~9.9 MB** | 기준 |
| **jcode** | **~10.4 MB** | **RAM 1.1배** |
| **pi** | **~76.5 MB** | **RAM 7.7배** |
| **Codex CLI** | **~21.6 MB** | **RAM 2.2배** |
| **OpenCode** | **~318.4 MB** | **RAM 32.2배** |
| **GitHub Copilot CLI** | **~158.1 MB** | **RAM 16.0배** |
| **Cursor Agent** | **~157.5 MB** | **RAM 15.9배** |
| **Claude Code** | **~212.7 MB** | **RAM 21.5배** |
| **Antigravity CLI** | **~86.4 MB** | **RAM 8.7배** |

</div>
이번에 보정된 메모리 재측정에 사용된 버전:

- `jcode v0.9.1888-dev (be386f2)`
- `pi 0.62.0`
- `codex-cli 0.120.0`
- `opencode 1.0.203`
- 1세션 재측정: `GitHub Copilot CLI 1.0.24`, 10세션 재측정: `GitHub Copilot CLI 1.0.27`
- `Cursor Agent 2026.04.08-a41fba1`
- `Claude Code 2.1.86 (Claude Code)`
- `Antigravity CLI 1.0.0`

<div align="center">

  <a href="https://github.com/1jehuang/jcode/releases/download/readme-assets/jcode-performance-demo.mp4">
    <img src="https://github.com/1jehuang/jcode/releases/download/readme-assets/jcode-performance-demo.webp" alt="jcode performance demonstration" width="900">
  </a>

  <p><em>jcode 성능 시연</em></p>

</div>


---

## 메모리 (에이전트 메모리)

Jcode는 매 턴/응답을 의미론적 벡터로 임베딩합니다. 매 턴마다 코사인 유사도 검사를 통해 관련된 메모리 항목을 효율적으로 찾기 위해 메모리 그래프를 질의합니다. 임베딩 히트는 대화에 주입되거나, 선택적으로 메모리 사이드에이전트가 해당 메모리가 관련성이 있는지 검증하고 대화에 주입하기 전에 정보 검색을 위한 추가 작업을 수행하기도 합니다. 이 결과 에이전트는 메모리 도구를 능동적으로 호출하거나 토큰을 낭비하지 않고도 대화와 관련된 정보를 자동으로 회상할 수 있는, 사람과 같은 메모리 시스템을 갖게 됩니다.

회상되는 메모리를 갖기 위해서는 먼저 추출되고 저장되어야 합니다. 일정 주기마다(의미론적 드리프트, 마지막 추출 이후 K턴 경과, 세션 종료 등) 메모리 사이드에이전트를 통해 메모리가 추출되어 메모리 그래프에 저장됩니다.

이 하네스는 또한 수동적인 백그라운드 프로세스에 의존하지 않고 에이전트가 능동적으로 메모리를 검색하거나 저장할 수 있도록 명시적인 메모리 도구를 제공합니다. 또한 이전 세션에 대한 전통적인 RAG를 위해 세션 검색 기능도 제공합니다.

메모리는 앰비언트 모드를 통해 일정 주기마다 자동으로 통합됩니다. 이 과정에서 메모리를 재구성하고, 오래된 정보와 충돌을 검사하는 등의 작업이 이루어집니다.

<div align="center">

  <a href="https://github.com/1jehuang/jcode/releases/download/readme-assets/jcode-memory-demo.mp4">
    <img src="https://github.com/1jehuang/jcode/releases/download/readme-assets/jcode-memory-demo.webp" alt="jcode memory demonstration" width="900">
  </a>

  <p><em>jcode 메모리 시연</em></p>

</div>

<!-- Memory demo media is hosted in the readme-assets release. -->

---

## UI: 사이드 패널, 다이어그램, 정보 위젯, 렌더링, 스크롤링, 정렬

사이드 패널은 보조 정보를 위한 공간입니다. jcode 에이전트에게 파일을 사이드 패널에 로드하도록 지시하면 실시간으로 갱신되는 것을 볼 수 있고, 에이전트가 사이드 패널에 직접 쓰도록 지시하거나 diff 뷰어로 사용할 수도 있습니다. 사이드 패널(그리고 채팅)은 mermaid 다이어그램을 인라인으로 렌더링할 수 있습니다.
<img width="2877" height="1762" alt="image" src="https://github.com/user-attachments/assets/6c7bec81-ef3f-434d-8a7b-d55f8a54e5cf" />

이를 가능하게 하기 위해, 다이어그램을 1800배 더 빠르게 렌더링하는 새로운 mermaid 렌더링 라이브러리를 만들었습니다. 브라우저나 Typescript 의존성이 전혀 없습니다. https://github.com/1jehuang/mermaid-rs-renderer 를 참고하세요.

응답에 사용할 수 있는 화면 공간을 빼앗지 않으면서 중요한 정보를 보여주기 위해 정보 위젯을 개발했습니다. 정보 위젯은 화면의 여백 공간만 사용해 정보를 표시하며, 여백이 없으면 알아서 사라집니다.

Jcode는 초당 천 프레임 이상으로 렌더링할 수 있습니다. 모니터의 주사율이 이를 모두 표시할 만큼 높지는 않겠지만, 이는 성가신 깜빡임 문제가 없다는 뜻입니다.

jcode의 커스텀 스크롤백 구현 덕분에 네이티브 스크롤백보다 훨씬 많은 것을 할 수 있습니다. 다만 부드럽고 부분적인 줄 단위 스크롤은 터미널 자체의 한계로 인해 커스텀 스크롤백으로 구현할 수 없었습니다. 이를 해결하기 위해 자체 터미널을 만들었습니다. Handterm(https://github.com/1jehuang/handterm)은 네이티브 스크롤 API를 구현하며, 동시에 매우 효율적입니다. 이는 아직 진행 중인 작업입니다. 일반 터미널에서의 스크롤링은 여전히 잘 구현되어 있습니다.

Jcode는 기본적으로 왼쪽 정렬입니다. `Alt+C` 단축키, `/alignment` 명령, 또는 설정을 통해 중앙 정렬 모드로 전환할 수 있습니다.

TUI와 CLI 출력에서 이모지를 전역적으로 비활성화하려면 `~/.jcode/config.toml`의 `[display]` 아래에 `emoji = false`를 설정하거나 `JCODE_NO_EMOJI=1`로 실행하세요. Jcode는 다른 유니코드 텍스트는 유지하면서 이모지를 간결한 ASCII 마커로 대체합니다.

---

## Swarm

같은 저장소에서 둘 이상의 에이전트를 실행하면, 서버가 자동으로 이들을 관리해 네이티브 협업이 가능해집니다. 에이전트 A가 에이전트 B가 읽은 파일을 편집하면(발밑에서 코드가 바뀌는 상황), 서버가 에이전트 B에게 알립니다. 에이전트 B는 관련이 없다면 무시할 수도 있고, diff를 확인해서 충돌이 없는지 점검할 수도 있습니다. 각 에이전트는 메시징 기능을 가지고 있어서, 단일 에이전트에게 DM을 보내거나, 서버가 호스팅하는 모든 에이전트에게 브로드캐스트하거나, 해당 저장소에서 작업 중인 에이전트에게만 전송할 수 있습니다. 이를 통해 같은 저장소에서 여러 세션을 실행하면서도 모든 충돌이 자동으로 해결되도록 할 수 있습니다.

<div align="center">

  <a href="https://github.com/1jehuang/jcode/releases/download/readme-assets/swarm-demo.mp4">
    <img src="https://github.com/1jehuang/jcode/releases/download/readme-assets/jcode-swarm-demonstration.webp" alt="jcode swarm demonstration" width="900">
  </a>

  <p><em>jcode swarm 시연</em></p>

</div>

에이전트는 스스로 자기만의 swarm을 자율적으로 생성할 수도 있습니다. 작업을 병렬로 수행하기 위해 팀원 에이전트를 스스로 생성하는 swarm 도구를 가지고 있습니다. 이렇게 하면 메인 에이전트는 코디네이터가 되고, 생성된 에이전트들은 워커가 됩니다. 에이전트 그룹, 메시징 채널, 완료 상태 등은 모두 자동으로 관리됩니다. 이는 헤드리스로도, 헤드가 있는 상태로도 수행할 수 있습니다.

---

## OAuth 및 프로바이더

jcode는 구독 기반 OAuth 플로우와 다양한 프로바이더 통합을 지원하므로, 이미 비용을 지불하고 있는 모델을 그대로 사용하면서도 필요할 때는 직접 API 프로바이더로 폴백할 수 있습니다.

### 지원되는 내장 로그인 플로우

- **Claude** (`jcode login --provider claude`)
- **OpenAI / ChatGPT / Codex** (`jcode login --provider openai`)
- **Google Gemini** (`jcode login --provider gemini`)
- **GitHub Copilot** (`jcode login --provider copilot`)
- **Azure OpenAI** (`jcode login --provider azure`)
- **Alibaba Cloud Coding Plan** (`jcode login --provider alibaba-coding-plan`)
- **Fireworks** (`jcode login --provider fireworks`)
- **MiniMax** (`jcode login --provider minimax`)
- **Meta Model API / Muse** (`jcode login --provider meta-muse`)
- **LM Studio** (`jcode login --provider lmstudio`)
- **Ollama** (`jcode login --provider ollama`)
- **커스텀 OpenAI 호환 엔드포인트** (`jcode login --provider openai-compatible`)

커스텀 OpenAI 호환 엔드포인트의 경우, jcode는 이제 API base를 물어보며 API 키 없이도 로컬 localhost 서버를 지원합니다.

### 셀프 호스팅 엔드포인트 및 MCP를 위한 설정 파일 구성

로그인 UI 대신 파일을 편집해서 설정하고 싶다면, jcode는 커스텀 OpenAI 호환 엔드포인트 설정과 MCP 설정 파일을 모두 지원합니다.

#### OpenAI 호환 프로바이더

많은 호스팅 서비스가 표준 OpenAI `/v1/chat/completions` API를 사용합니다. jcode는 하나의 공유 OpenAI 호환 프로바이더를 통해 이들과 통신하므로, 전용 통합을 기다리지 않고도 거의 모든 이런 엔드포인트를 사용할 수 있습니다.

설정하는 방법은 두 가지입니다:

- **내장된 이름 지정 프로필** — jcode는 여러 인기 있는 OpenAI 호환 서비스용 준비된 프로필을 제공합니다. id로 로그인하면 jcode가 base URL과 키 환경 변수를 자동으로 채워줍니다:

  ```bash
  jcode login --provider <profile-id>
  # for example:
  jcode login --provider openrouter
  jcode login --provider orcarouter
  jcode login --provider deepseek
  jcode login --provider opencode      # OpenCode Zen
  jcode login --provider moonshotai
  jcode login --provider meta-muse     # Meta Model API / Muse Spark
  ```

  내장 OpenAI 호환 프로필 id에는 `openrouter`, `orcarouter`, `deepseek`, `zai`, `kimi`, `moonshotai`, `meta-muse`(Meta Model API / Muse Spark), `opencode`(OpenCode Zen), `opencode-go`, `302ai`, `baseten`, `cortecs`, `huggingface`, `nebius`, `scaleway`, `stackit`, `firmware`가 포함됩니다. 각 프로필은 엔드포인트와 키 변수만 설정하며, 모델은 여전히 `/model`(또는 `--model`)로 직접 선택해야 합니다. 프로바이더를 지정하지 않고 `jcode login`을 실행하면 대화형 목록을 볼 수 있습니다.

- **그 외 모든 엔드포인트** — `jcode login --provider openai-compatible` 또는 아래 설명된 스크립트 가능한 `jcode provider add` 명령으로 임의의 OpenAI 호환 API(호스팅형 또는 로컬)를 가리킬 수 있습니다.

이런 엔드포인트에 유용한 환경 변수 오버라이드:

- `JCODE_STREAM_IDLE_TIMEOUT_SECS` — 토큰을 내보내기 전 조용히 생각하는 느린 추론 모델을 위해 기본 스트리밍 idle 타임아웃(기본 180초)을 늘립니다. 높은 추론 강도는 이를 자동으로 스케일링합니다(high 2배, xhigh 3배, max 4배). `config.toml`에서 `[provider] stream_idle_timeout_secs`로도 설정할 수 있습니다.
- `[[providers.<name>.models]]` 항목의 모델별 `context_window`(별칭 `context_limit`) — 엔드포인트가 사용 가능한 `/v1/models` 응답을 제공하지 않을 때 컨텍스트 윈도우를 설정하여, jcode가 일반적인 200k 기본값으로 폴백하지 않도록 합니다.
- `extra_body` — 이런 필드를 요구하는 백엔드를 위해 모든 chat/completions 요청 본문에 비표준 최상위 필드를 주입합니다. 아래 [추가 요청 본문 필드](#extra-request-body-fields-extra_body) 섹션을 참고하세요.

셀프 호스팅, 로컬 런타임, 정확한 설정 파일 형식에 대한 자세한 내용은 아래를 참고하세요.

#### vLLM을 포함한 셀프 호스팅 OpenAI 호환 엔드포인트

에이전트와 스크립트의 경우, 권장되는 방법은 원샷 프로바이더 프로필 명령입니다. 이 명령은 `~/.jcode/config.toml`에 이름 지정 프로필을 기록하고, 요청 시 jcode의 비공개 앱 설정 디렉터리에 시크릿을 저장하며, 정확한 실행/검증 명령을 출력합니다:

```bash
# Secret-safe setup for a hosted OpenAI-compatible API.
printf '%s' "$MY_API_KEY" | jcode provider add my-api \
  --base-url https://llm.example.com/v1 \
  --model my-model-id \
  --api-key-stdin \
  --set-default \
  --json

# Smoke test the profile.
jcode --provider-profile my-api auth-test --prompt 'Reply exactly JCODE_PROVIDER_SETUP_OK'

# Use it directly.
jcode --provider-profile my-api run 'hello'
```

인증이 필요 없는 로컬 서버의 경우:

```bash
jcode provider add local-vllm \
  --base-url http://localhost:8000/v1 \
  --model Qwen/Qwen3-Coder-30B-A3B-Instruct \
  --no-api-key \
  --set-default
```

일반적인 데스크톱/로컬 런타임에는 내장 로컬 프로필을 사용할 수 있습니다:

```bash
# Ollama: start the local server and install a model first.
ollama pull llama3.2
jcode login --provider ollama
jcode --provider ollama --model llama3.2 run 'hello'

# LM Studio: start the Local Server, load a chat model, then use the exact
# model identifier shown by LM Studio or by curl http://localhost:1234/v1/models.
jcode login --provider lmstudio
jcode --provider lmstudio --model '<model-id>' run 'hello'
```

Ollama와 LM Studio는 모두 OpenAI 호환 `/v1/models` 및 `/v1/chat/completions` 엔드포인트를 제공합니다. jcode는 비전 지원 로컬 모델에 대해 스트리밍 chat completions, 함수/도구 호출, OpenAI 스타일 이미지 콘텐츠를 사용합니다. 로컬 서버가 토큰을 요구하는 경우, `jcode login` 중에 입력하거나 `--api-key-stdin`으로 이름 지정 프로필을 생성하세요.

유용한 플래그:

- `--api-key-env NAME`: 키를 저장하는 대신 기존 환경 변수를 참조합니다.
- `--api-key-stdin`: 셸 히스토리에 남기지 않고 키를 읽어서 저장합니다.
- `--context-window TOKENS`: 모델 선택과 라우팅을 위해 모델 컨텍스트 윈도우를 영속화합니다.
- `--overwrite`: 동일한 이름의 기존 프로필을 대체합니다.
- `--model-catalog`: 설정된 모델 외에도 엔드포인트의 `/models` 응답을 사용합니다.

생성된 프로필은 `~/.jcode/config.toml`에서 수동으로 편집할 수도 있습니다:

```toml
[provider]
default_provider = "my-api"
default_model = "my-model-id"

[providers.my-api]
type = "openai-compatible"
base_url = "https://llm.example.com/v1"
api_key_env = "JCODE_PROVIDER_MY_API_API_KEY"
env_file = "provider-my-api.env"
default_model = "my-model-id"
# Optional: prevent model names such as `gpt-5-*` from automatically enabling
# `reasoning_effort` on gateways that reject it.
disable_reasoning_heuristics = true

[[providers.my-api.models]]
id = "my-model-id"
context_window = 128000
# Explicitly enable `/effort` and select this model's initial effort. Set
# `reasoning = false` on an individual model to disable it instead.
reasoning = true
reasoning_effort = "high"
```

Anthropic Messages 호환 게이트웨이는 `type = "anthropic-compatible"`을 사용하는 동일한 이름 지정 프로필 방식을 사용합니다. 이 프로필은 bearer, 커스텀 헤더, 또는 인증 없음 중 선택할 수 있으며 게이트웨이별 헤더를 모든 요청에 첨부할 수 있습니다:

```toml
[provider]
default_provider = "corp-claude"
default_model = "claude-sonnet-4-6"

[providers.corp-claude]
type = "anthropic-compatible"
base_url = "https://gateway.example.com/anthropic/v1"
auth = "bearer"
api_key_env = "CORP_CLAUDE_TOKEN"
default_model = "claude-sonnet-4-6"

[providers.corp-claude.headers]
x-tenant-id = "tenant-42"

[[providers.corp-claude.models]]
id = "claude-sonnet-4-6"
context_window = 200000
```

직접 환경 변수 기반 설정을 사용하는 경우, `ANTHROPIC_BASE_URL`이 OAuth가 아닌 Messages 엔드포인트를 오버라이드하며 `ANTHROPIC_AUTH_TOKEN`이 bearer 토큰으로 전송됩니다.
Claude OAuth 트래픽은 언제나 Anthropic의 공식 엔드포인트를 계속 사용합니다.

##### 추가 요청 본문 필드 (`extra_body`)

일부 OpenAI 호환 백엔드는 비표준 최상위 요청 필드를 요구합니다. 예를 들어 NVIDIA NIM DeepSeek-V4 추론 모델(`deepseek-ai/deepseek-v4-flash`, `deepseek-ai/deepseek-v4-pro`)은 요청에 `chat_template_kwargs`가 포함될 때만 thinking을 활성화합니다. 없으면 추론 없이 응답하거나(일부 배포에서는 멈춰버립니다), jcode는 두 가지 방법으로 임의의 최상위 필드를 주입할 수 있게 해줍니다.

1. `config.toml`의 `extra_body`를 통해 이름 지정 프로필별로 설정(JSON 본문에 그대로 병합되는 TOML 테이블):

   ```toml
   [providers.my-nim]
   type = "openai-compatible"
   base_url = "https://integrate.api.nvidia.com/v1"
   api_key_env = "NVIDIA_API_KEY"
   default_model = "deepseek-ai/deepseek-v4-flash"

   [providers.my-nim.extra_body.chat_template_kwargs]
   thinking = true
   reasoning_effort = "high"
   ```

2. 내장 프로필(예: `nvidia-nim`) 또는 모든 엔드포인트의 경우, `JCODE_OPENAI_EXTRA_BODY` 환경 변수(JSON 객체 문자열)를 통해 설정. API 키 옆의 프로바이더 env 파일(`~/.config/jcode/nvidia-nim.env`)에 함께 둘 수 있습니다:

   ```bash
   JCODE_OPENAI_EXTRA_BODY={"chat_template_kwargs":{"thinking":true,"reasoning_effort":"high"}}
   ```

`extra_body`의 키는 마지막에 병합되어 동일한 이름의 jcode 생성 본문 필드를 오버라이드합니다(키가 충돌할 경우 `JCODE_OPENAI_EXTRA_BODY`가 설정 파일의 `extra_body`보다 우선합니다). 잘못된 값은 요청을 실패시키는 대신 로그에 남기고 무시됩니다.

커스텀 OpenAI 호환 프로바이더는 환경 변수 또는 jcode의 앱 설정 디렉터리에 있는 env 파일에서 오버라이드를 읽습니다. Linux에서는 보통 `~/.config/jcode/`이므로, 기본 파일은 보통 다음과 같습니다:

```text
~/.config/jcode/openai-compatible.env
```

로컬 또는 LAN vLLM 서버의 예시:

```bash
JCODE_OPENAI_COMPAT_API_BASE=http://192.168.1.50:8000/v1
JCODE_OPENAI_COMPAT_DEFAULT_MODEL=Qwen/Qwen3-Coder-30B-A3B-Instruct
# Optional if your server expects auth
OPENAI_COMPAT_API_KEY=your-token-here
```

참고:

- `jcode login --provider openai-compatible`이 이 파일을 대신 생성하거나 갱신해줄 수 있습니다.
- `localhost`와 사설 LAN IP에 대해서는 일반 `http://`가 허용됩니다. 공개 원격 HTTP는 여전히 거부됩니다.
- HTTPS 엔드포인트는 평소처럼 동작합니다.

#### MCP 설정 파일

MCP 설정은 `config.toml`과 별도입니다.

기본 설정 파일:

- 전역 MCP 서버는 `~/.jcode/mcp.json`
- 프로젝트 로컬 MCP 서버는 `.jcode/mcp.json`

Claude Code 호환성:

- `~/.claude.json`(Claude Code의 사용자 설정): 최상위 `mcpServers`와, 현재 디렉터리에 대해 `projects.<abs_path>.mcpServers` 아래의 프로젝트별 서버
- 저장소 루트의 `.mcp.json`(Claude Code의 프로젝트 설정)
- `.claude/mcp.json`(레거시 폴백)

Claude Code 설정은 jcode의 전역 설정에 복사되는 대신 로드될 때마다 실시간으로 읽힙니다. 따라서 추가, 수정, 삭제가 오래된 스냅샷을 남기지 않고 즉시 반영됩니다(인라인 환경 값도 중복 저장되지 않습니다).
Codex CLI로부터의 마이그레이션을 위해, jcode는 `~/.jcode/mcp.json`이 존재하지 않을 때 `~/.codex/config.toml`에서 한 번만 임포트를 수행합니다.
이렇게 임포트된 파일은 이후 jcode가 소유하게 되며, 이후의 Codex 변경 사항은 자동으로 동기화되지 않습니다. 환경 값도 함께 복사되므로 시크릿이 포함될 수 있습니다.

표준 `mcpServers` 키와 jcode의 기존 `servers` 키 모두 허용됩니다. jcode는 현재 stdio(명령 기반) 서버만 지원하며, HTTP/SSE 항목(`"type": "http"`/`"sse"`)은 인식은 되지만 로그 한 줄과 함께 건너뜁니다.

MCP 설정 예시:

```json
{
  "mcpServers": {
    "filesystem": {
      "command": "/path/to/mcp-server",
      "args": ["--root", "/workspace"],
      "env": {},
      "shared": true
    }
  }
}
```

헤드리스 또는 SSH 세션의 경우, OAuth 방식 프로바이더는 `jcode login --provider <provider> --no-browser`(별칭: `--headless`)를 지원하므로 jcode가 로컬 브라우저를 실행하는 대신 인증 URL/QR을 출력하고 수동 코드나 콜백 붙여넣기로 폴백합니다.

더 스크립트 가능한 원격 플로우를 위해, `claude`, `openai`, `gemini`, `antigravity`도 2단계 패턴을 지원합니다:

```bash
# Step 1: print a resumable auth URL
jcode login --provider openai --print-auth-url --json

# Step 2: complete later with the callback URL or auth code
jcode login --provider openai --callback-url 'http://localhost:1455/auth/callback?...'
jcode login --provider gemini --auth-code '...'
```

추가로 스크립트로 처리 가능한 경우:

```bash
# Copilot device flow: print URL + user code, then complete later
jcode login --provider copilot --print-auth-url --json
jcode login --provider copilot --complete

# Gmail/Google OAuth after credentials are already configured
jcode login --provider google --print-auth-url --google-access-tier readonly
jcode login --provider google --callback-url 'http://127.0.0.1:8456?...'
```

대기 중인 스크립트 로그인 상태는 `~/.jcode/pending-login/` 아래에 저장되며, 자동으로 만료되고, 새 스크립트 로그인이 시작되거나 재개될 때 오래된 항목이 정리됩니다.

내장 OpenAI 로그인 플로우의 경우, jcode는 기본적으로 `http://localhost:1455/auth/callback`에 로컬 콜백을 엽니다.

<img width="2877" height="1762" alt="Screenshot from 2026-04-02 14-28-51" src="https://github.com/user-attachments/assets/530684c0-9d12-4363-aa0e-1b39a0d4e1be" />
위 이미지는 프로바이더 로그인의 첫 페이지입니다

### 지원되는 프로바이더

- **네이티브 / 퍼스트파티 방식 프로바이더:** `claude`, `openai`, `copilot`, `gemini`, `azure`, `alibaba-coding-plan`
- **애그리게이터 / 호환 프로바이더:** `openrouter`, `orcarouter`, `openai-compatible`
- **추가 프로바이더 통합:** `opencode`, `opencode-go`, `zai` / `kimi`, `302ai`, `baseten`, `cortecs`, `deepseek`, `firmware`, `huggingface`, `moonshotai`, `nebius`, `scaleway`, `stackit`, `groq`, `mistral`, `perplexity`, `togetherai`, `deepinfra`, `fireworks`, `minimax`, `xai`, `lmstudio`, `ollama`, `chutes`, `cerebras`, `cursor`, `antigravity`, `google`

Jcode는 손쉬운 멀티 계정 전환도 지원합니다. 첫 번째 ChatGPT Pro 구독의 토큰을 다 썼나요? /account로 두 번째 계정으로 빠르게 전환하세요.

---

## 커스터마이징 / 셀프 개발

Jcode는 플러그인이나 확장이 할 수 있는 범위에 국한되지 않는 새로운 형태의 커스터마이징을 만들어가고 있습니다. jcode 에이전트에게 셀프 개발 모드에 진입하라고 지시하면, 자기 자신의 소스 코드를 수정하기 시작합니다. Jcode는 스스로를 개선(iterate)하도록 최적화되어 있습니다. 자기 자신의 소스 코드를 편집·빌드·테스트한 다음 자체 바이너리를 리로드하고 여러분의 (동시에 여러 개일 수 있는) 세션에서 완전히 자동으로 작업을 계속할 수 있도록 하는 상당한 규모의 셀프 개발 인프라가 갖춰져 있습니다.

이 작업에는 프론티어 모델을 사용하는 것을 권장합니다. jcode 코드베이스는 단순하지 않으며, 약한 모델은 미묘하지만 치명적인 변경을 만들 수 있습니다. GPT 5.5나 사용 가능한 최신 프론티어 모델이 잘 작동합니다.

<!-- Add self-dev demo thumbnail/video and fuller writeup here. -->

---

## 기타

디테일에 진리가 있습니다. jcode에는 문서화되지 않은 다양한 최적화와 편의 기능이 많이 구현되어 있습니다. 몇 가지 예시:

Anthropic의 Claude 캐시는 5분 후에 식습니다(cold). 이 5분이 지난 후 Claude를 호출하면 캐시 미스가 발생해 많은 토큰 비용이 들 수 있습니다. UI는 캐시가 식었을 때 경고를 표시하고, 예상치 못한 캐시 미스가 발생했을 때 알려줍니다.

jcode는 Firefox Agent Bridge를 설정하는 방법에 대한 안내가 함께 제공됩니다. 에이전트에게 설정을 요청하면 jcode에서도 브라우저 자동화를 사용할 수 있게 됩니다.

Agent grep은 jcode 에이전트를 위해 만든 grep 도구입니다. grep 결과에 파일 구조 정보(예: 함수 목록, 위치 등)를 추가해서, 에이전트가 파일을 실제로 읽지 않고도 파일이 무엇을 하는지 더 많이 추론할 수 있게 해줍니다. 또한 에이전트가 이미 본 내용을 기반으로 결과를 적응적으로 잘라내는 하네스 레벨 통합도 구현되어 있습니다. 이는 컨텍스트를 크게 절약해줍니다.

입력은 기본적으로 작업 중인 에이전트와 인터리브됩니다. KV 캐시를 깨뜨리지 않고 안전하게 보낼 수 있는 즉시 입력을 전송합니다. Shift+Enter로 제출하면 큐 전송이 되어, 에이전트가 현재 턴을 완전히 마칠 때까지 기다렸다가 전송합니다.

다른 하네스에서 세션을 재개할 수 있습니다. Claude Code가 먹통이 되었나요? jcode에서 세션을 재개해서 하던 작업을 이어가세요. 세션 재개는 codex, claude code, opencode, pi에 대해 지원됩니다.

<img width="2877" height="1762" alt="Screenshot from 2026-04-11 16-28-52" src="https://github.com/user-attachments/assets/c2b383cf-2531-4217-85ae-6a863354dc97" />
codex 세션용 /Resume 이미지


스킬은 시작 시 전부 로드되지 않습니다. 대화는 의미론적 벡터로 임베딩되며, 메모리와 유사한 임베딩 히트가 있으면 자동으로 스킬을 주입합니다. 에이전트는 언제든 스킬을 수동으로 활성화할 수 있는 스킬 도구를 가지고 있습니다. 슬래시 명령으로도 활성화할 수 있습니다.

---

## iOS 애플리케이션 / 네이티브 OpenClaw

jcode의 네이티브 iOS 애플리케이션 버전이 곧 출시됩니다. 이를 통해 Tailscale을 경유해 여러분의 휴대폰에서 개인 컴퓨터 환경의 jcode와 함께 작업할 수 있게 됩니다. Openclaw와 유사한 기능들이 이 iOS 애플리케이션에 번들로 제공될 예정입니다.

---

## 향후 계획 중인 기능

에이전트는 활성 변경 사항이 있는 더티(dirty)한 git 상태에서 커밋하는 것을 좋아하지 않습니다. Git은 명백히 멀티 에이전트 워크플로우를 위해 만들어지지 않았고, git worktree도 좋은 해결책은 아닙니다. 이를 고려할 때, 새로운 git과 유사한 프리미티브가 탄생할 기회가 있다고 생각합니다.

빌드 속도 개선: 캐시가 활성화된 증분 디버그 cargo 빌드는 제 머신에서 약 1분이 걸립니다. 목표는 5-20초입니다. 리팩터링과 크레이트 경계 재정비를 통해 이를 달성할 수 있을 것입니다.

<!-- Add iOS / native OpenClaw preview and fuller writeup here. -->

---

<div align="center">

## 빠른 시작

</div>

```bash
# Launch the TUI
jcode

# Run a single command non-interactively
jcode run "say hello"

# Resume a previous session by memorable name
jcode --resume fox

# Run as a persistent background server, then attach more clients
jcode serve
jcode connect

# Send voice input from your configured STT command
jcode dictate
```

jcode는 대화형 TUI 사용, 비대화형 실행, 영속적인 서버/클라이언트 워크플로우를 지원하며,
번들로 제공되는 음성 인식 스택 없이도 단축키 친화적인 받아쓰기를 지원합니다.

<div align="center">

  <a href="https://github.com/1jehuang/jcode/releases/download/readme-assets/workflow.mp4">
    <img src="https://github.com/1jehuang/jcode/releases/download/readme-assets/jcode-workflow-demonstration.webp" alt="jcode workflow demonstration" width="900">
  </a>

  <p><em>jcode 워크플로우 시연</em></p>

</div>

---

## 브라우저 자동화

jcode는 에이전트 세션 내에서 브라우저를 제어할 수 있는 퍼스트클래스 내장 `browser` 도구를 포함합니다.

현재 내장된 백엔드:
- Firefox Agent Bridge를 통한 Firefox

현재 내장된 도구 액션:
- `status`
- `setup`
- `open`
- `snapshot`
- `get_content`
- `interactables`
- `click`
- `type`
- `fill_form`
- `select`
- `wait`
- `screenshot`
- `eval`
- `scroll`
- `upload`
- `press`

빠른 설정:

```bash
jcode browser status
jcode browser setup
```

설정이 완료되면, 모델은 내장 `browser` 도구를 직접 사용할 수 있습니다. UI는 또한 URL 열기, 셀렉터 클릭, 필드에 입력하는 등의 브라우저 도구 호출을 민감하게 입력된 텍스트를 에코하지 않으면서 간결하게 요약해서 보여줍니다.

참고:
- 프로바이더/도구 아키텍처는 추가 백엔드를 위해 이미 갖춰져 있습니다
- 현재 연결된 내장 백엔드는 Firefox입니다
- Chrome bridge / 원격 디버깅 스타일의 프로바이더도 나중에 동일한 browser 도구 위에 추가될 수 있습니다

---

## 더 읽어보기

- [jcode.sh/docs](https://jcode.sh/docs) — 설치, 프로바이더, 설정, 키바인딩
- [jcode.sh/swarm](https://jcode.sh/swarm) — 하나의 저장소에서 여러 코딩 에이전트 사용하기
- [jcode.sh/sdk](https://jcode.sh/sdk) — TypeScript SDK: 여러분만의 프로그램에서 jcode 세션을 구동하기
- [jcode.sh/bench](https://jcode.sh/bench) — 벤치마크 방법론 및 결과
- [Ambient Mode / OpenClaw](docs/AMBIENT_MODE.md)
- [Browser Provider Protocol](docs/BROWSER_PROVIDER_PROTOCOL.md)
- [Memory Architecture](docs/MEMORY_ARCHITECTURE.md)
- [Swarm Architecture](docs/SWARM_ARCHITECTURE.md)
- [Server Architecture](docs/SERVER_ARCHITECTURE.md)
- [Safety System](docs/SAFETY_SYSTEM.md)
- [Sponsored Discovery Sponsor Onboarding](docs/SPONSORED_DISCOVERY_SPONSOR_ONBOARDING.md)
- [Windows Notes](docs/WINDOWS.md)
- [Wrappers and Shell Integration](docs/WRAPPERS.md)
- [Refactoring Notes](docs/REFACTORING.md)

---

## 상세 설치

### 설정

다른 에이전트가 대신 jcode를 설정해주길 원한다면, 다음 프롬프트를 전달하세요:

```text
Set up jcode on this machine for me.

1. Detect the operating system, available package managers, and shell environment, then install jcode using the best matching command below instead of referring me somewhere else:

   - macOS with Homebrew available:
     brew tap 1jehuang/jcode
     brew install jcode

   - macOS or Linux via install script:
     curl -fsSL https://jcode.sh/install | bash

   - Windows PowerShell:
     irm https://jcode.sh/install.ps1 | iex

   - From source if the above paths are not appropriate:
     git clone https://github.com/1jehuang/jcode.git
     cd jcode
     cargo build --release
     scripts/install_release.sh

   - For local self-dev / refactor work on Linux x86_64, prefer:
     scripts/dev_cargo.sh build --release -p jcode --bin jcode
     scripts/dev_cargo.sh --print-setup
     scripts/install_release.sh

2. Verify that `jcode` is on my `PATH`.
3. Launch `jcode` once in a new terminal window/session to confirm it starts successfully.
4. Before attempting any interactive login flow, assess which providers are already available non-interactively and prefer those first. Check existing local credentials, config files, CLI sessions, and environment variables such as:
   - Claude: `~/.jcode/auth.json`, `~/.claude/.credentials.json`, `~/.local/share/opencode/auth.json`, `ANTHROPIC_API_KEY`
   - OpenAI: `~/.jcode/openai-auth.json`, `~/.codex/auth.json`, `OPENAI_API_KEY`
   - Gemini: `~/.jcode/gemini_oauth.json`, `~/.gemini/oauth_creds.json`
   - GitHub Copilot: existing auth under `~/.config/github-copilot/`
   - Azure OpenAI: `~/.config/jcode/azure-openai.env`, `AZURE_OPENAI_*`, or an existing `az login`
   - OpenRouter: `OPENROUTER_API_KEY`
   - Fireworks: `~/.config/jcode/fireworks.env`, `FIREWORKS_API_KEY`
   - MiniMax: `~/.config/jcode/minimax.env`, `MINIMAX_API_KEY`
   - NVIDIA NIM: `~/.config/jcode/nvidia-nim.env`, `NVIDIA_API_KEY`
   - Alibaba Cloud Coding Plan: existing jcode config/env if present
5. Prefer whichever provider is already configured and verify it with `jcode auth-test --all-configured` or a provider-specific auth test when appropriate.
6. Only if no usable provider is already configured, guide me through the minimal manual step needed:
   - Claude: `jcode login --provider claude`
   - GitHub Copilot: `jcode login --provider copilot`
   - OpenAI: `jcode login --provider openai`
   - Gemini: `jcode login --provider gemini`
   - Azure OpenAI: `jcode login --provider azure`
   - Fireworks: `jcode login --provider fireworks`
   - MiniMax: `jcode login --provider minimax`
   - NVIDIA NIM: `jcode login --provider nvidia-nim`
   - Alibaba Cloud Coding Plan: `jcode login --provider alibaba-coding-plan`
   - OpenRouter: help me set `OPENROUTER_API_KEY`
   - Anthropic direct API: help me set `ANTHROPIC_API_KEY`
7. After setup, run a simple smoke test with `jcode run "say hello"` and confirm it works.
8. If I want browser automation, also check `jcode browser status`. If browser automation is not ready, run `jcode browser setup`, verify the built-in `browser` tool works, and explain any remaining manual step.
9. Explain any manual step that still needs me, especially browser OAuth, device login, API key entry, or browser extension approval.
```

이는 jcode 자체 또는 다른 코딩 에이전트를 위한 복사-붙여넣기용 부트스트랩 프롬프트로 의도된 것입니다.

### 빠른 설치

```bash
# macOS & Linux
curl -fsSL https://jcode.sh/install | bash
```

Termux에서는 먼저 glibc 런타임과 `patchelf`를 설치해야 설치 스크립트가 다운로드한 Linux 바이너리를
Termux의 glibc 동적 링커에 맞게 패치하고, Termux의 `LD_PRELOAD` 셈을 우회하는 런처를 만들 수 있습니다:

```bash
pkg install glibc patchelf
curl -fsSL https://jcode.sh/install | bash
```

```powershell
# Windows 11 x64 or ARM64 (PowerShell 5.1+)
irm https://jcode.sh/install.ps1 | iex
```

Windows 설치 스크립트는 올바른 아키텍처를 선택하고 릴리스의 `SHA256SUMS`로 다운로드를 검증합니다.
Alacritty와 선택적인 전역 실행 단축키는 명시적인 동의가 필요하며 기본적으로는 설치되지 않습니다.
[Windows 지원, 보안, Defender, SmartScreen 관련 참고 사항](docs/WINDOWS.md)을 참고하세요.

릴리스에 일치하는 Windows 에셋이 없으면, 설치 스크립트는 예상치 못한 긴 컴파일을 시작하는 대신 중단됩니다.
`-BuildFromSource`를 통해 명시적인 소스 빌드를 사용할 수 있으며, 이 경우 Git, Rust, **Desktop development with C++** 워크로드가 포함된 Visual Studio 2022 Build Tools가 필요합니다.

### macOS (Homebrew 사용)

```bash
brew tap 1jehuang/jcode
brew install jcode
```

### 소스에서 빌드 (모든 플랫폼)

```bash
git clone https://github.com/1jehuang/jcode.git
cd jcode
cargo build --release
```

Linux x86_64에서 로컬 셀프 개발 / 리팩터링 작업을 하는 경우 다음을 권장합니다:

```bash
scripts/dev_cargo.sh build --release -p jcode --bin jcode
scripts/dev_cargo.sh --print-setup
```

이 래퍼는 가능한 경우 자동으로 `sccache`를 사용하며, 모든 머신의 `mold` 설정이 유효하다고 가정하는 대신
빠르게 동작하는 로컬 링커 설정(`clang + lld`)을 우선 사용합니다. 또한 `--print-setup`으로 현재 활성화된
링커/캐시 설정을 출력해서 느린 빌드 경로를 더 쉽게 진단할 수 있게 해줍니다.

그런 다음 PATH에 심볼릭 링크를 생성하세요:

```bash
scripts/install_release.sh
```

### 제거

설치된 바이너리와 런처를 제거하지만, 설정·인증·세션은 그대로 유지해서 깨끗하게 재설치해도
하던 작업을 이어갈 수 있습니다:

```bash
curl -fsSL https://raw.githubusercontent.com/1jehuang/jcode/master/scripts/uninstall.sh | bash -s -- --yes
```

설정, 인증, 세션, 로그, 메모리를 포함한 모든 것을 완전히 지우려면(깨진 설치를 복구할 때 유용):

```bash
curl -fsSL https://raw.githubusercontent.com/1jehuang/jcode/master/scripts/uninstall.sh | bash -s -- --purge --yes
```

`--dry-run`을 추가하면 실제로 삭제하지 않고 무엇이 제거될지 미리 볼 수 있습니다.

### 플랫폼 지원

| 플랫폼 | 상태 |
|---|---|
| **Linux** x86_64 / aarch64 | 완전 지원 |
| **macOS** Apple Silicon & Intel | 지원 |
| **Windows** x86_64 | 지원 (네이티브 + WSL2) |
| **Termux** aarch64 / x86_64 | `pkg install glibc patchelf`와 함께 지원 |

</div>
</content>
