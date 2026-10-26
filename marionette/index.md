---
title: Marionette MCP
---

# Marionette MCP

**Let your AI client see and operate Windows desktop apps.** · by Sewoong Oh (RadishCode Labs)

[한국어](#ko) · [Privacy Policy](privacy) · Support: kumting1103@gmail.com

Marionette MCP is a local MCP server for Windows. An AI client such as Claude Code calls its tools to capture the screen, read text, find buttons and icons, and click or type in desktop apps — including apps that have no API.

## Features

- **Sees the screen**: text recognition (OCR, Korean and English) and icon detection run on your PC; elements come back as a numbered list.
- **Operates apps**: clicks, typing (Korean too), keys, scrolling, drag, window focus and placement, UI Automation when an app offers it.
- **Shows what it does**: a pointer and target highlight on screen, and an emergency stop (Ctrl+Alt+Q or a screen corner) that halts all input at once.
- **Learns apps**: short app notes (tips and pitfalls) it shares with the AI client the next time.
- **Works without administrator rights**: runs as a normal user; restart it as administrator from the tray menu when an app running as administrator must be driven.
- **Remote use (optional)**: let Claude Code on another PC you specify drive this one (a test VM, for example), with an access token and a firewall rule for that address only.

## Get it

- **Microsoft Store**: *Marionette MCP* (link after publication). Free, with a Pro add-on that removes the hourly limit.
- **Direct edition** for organizations that can't use the Microsoft Store: contact us.

## Connect Claude Code

After Marionette starts (tray icon), register it once in Claude Code:

```
claude mcp add --transport http marionette http://127.0.0.1:5300 -s user
```

Then restart Claude Code.

## Free and Pro

- **Free**: 100 tool calls in any one-hour window.
- **Pro**: no limit. Buy the Pro add-on in the Store, or enter a license key in the direct edition.

## Support

kumting1103@gmail.com

---

# Marionette MCP (한국어) {#ko}

**AI 클라이언트가 Windows 데스크톱 앱을 보고 조작하게 합니다.** · 오세웅(RadishCode Labs)

[개인정보 처리방침](privacy#ko) · 지원: kumting1103@gmail.com

Marionette MCP는 Windows용 로컬 MCP 서버입니다. Claude Code 같은 AI 클라이언트가 도구를 불러 화면을 캡처하고, 글자를 읽고, 버튼과 아이콘을 찾고, 데스크톱 앱을 클릭하거나 입력합니다. API가 없는 앱도 다룰 수 있습니다.

## 기능

- **화면 보기**: 글자 인식(OCR, 한국어·영어)과 아이콘 탐지를 PC 안에서 하고, 요소를 번호 목록으로 돌려줍니다.
- **앱 조작**: 클릭, 입력(한글 포함), 키, 스크롤, 드래그, 창 포커스·배치, 앱이 제공하면 UI Automation.
- **동작이 보임**: 화면에 포인터와 대상 강조를 표시하고, 긴급 정지(Ctrl+Alt+Q 또는 화면 모서리)로 모든 입력을 한 번에 멈춥니다.
- **앱을 배움**: 앱마다 짧은 노트(요령·함정)를 남겨 다음에 AI 클라이언트에 알려 줍니다.
- **관리자 권한 없이 동작**: 일반 사용자 권한으로 돌고, 관리자 권한 앱을 다뤄야 할 때 트레이 메뉴에서 관리자 권한으로 다시 시작합니다.
- **원격 사용(선택)**: 지정한 다른 PC의 Claude Code가 이 PC를 사용하게 합니다(예: 테스트 VM). 접속 토큰과 그 주소만 여는 방화벽 규칙을 씁니다.

## 받기

- **Microsoft Store**: *Marionette MCP*(게시 뒤 링크). 무료이고, 시간당 한도를 없애는 Pro 추가 기능이 있습니다.
- **직접 계약판**: Microsoft Store를 쓸 수 없는 조직용. 문의해 주세요.

## Claude Code 연결

Marionette가 시작되면(트레이 아이콘) Claude Code에 한 번 등록합니다.

```
claude mcp add --transport http marionette http://127.0.0.1:5300 -s user
```

그다음 Claude Code를 다시 시작합니다.

## Free와 Pro

- **Free**: 어느 1시간 동안이든 도구 호출 100회.
- **Pro**: 한도 없음. Store에서 Pro 추가 기능을 사거나, 직접 계약판에서 라이선스 키를 입력합니다.

## 지원

kumting1103@gmail.com
