---
title: Marionette MCP — Privacy Policy
---

# Marionette MCP — Privacy Policy

Effective date: 2026-10-26 · Developer: Sewoong Oh (RadishCode Labs) · Contact: kumting1103@gmail.com

[한국어는 아래에 있습니다.](#ko)

Marionette MCP ("Marionette") is a Windows desktop app that lets an AI client you run, such as Claude Code, see the screen and operate desktop apps on your PC through the Model Context Protocol (MCP). This policy explains what Marionette does with information on your PC.

## Summary

- Marionette has **no account, no analytics and no telemetry**. The developer does not receive your screen, your text, your files or your usage.
- Screen capture, text recognition (OCR) and screen analysis run **on your PC**.
- Results go **only to the AI client you connected** to Marionette. What happens after that is governed by that client and the AI service behind it.

## What Marionette processes

| Information | What happens to it |
| --- | --- |
| Screen contents (screenshots of the screen, a window or a region) | Captured when the AI client calls a tool. Analyzed on your PC (text recognition, icon detection, Windows UI Automation names). Kept in memory for the current session and not written to disk. |
| Recognized text, element lists, window titles and app names | Returned to the connected AI client as the tool's result. |
| Screenshots | Returned to the AI client only when it asks for an image. |
| Text the AI client types | Sent to the target app as keyboard input. To enter some text (such as Korean), Marionette puts it on the clipboard briefly, pastes it, and puts back the clipboard text that was there before. |
| Your own keyboard input | **Not recorded.** Marionette registers one global hotkey (the emergency stop, Ctrl+Alt+Q by default) and does not log other keys. |

## Where the results go

- **This PC (default):** the AI client connects to Marionette at `127.0.0.1` (only programs on this PC can reach it). Results stay on your PC until your AI client sends them to its AI service, under that service's own privacy policy (for Claude Code, Anthropic's).
- **Remote use (off by default):** if you turn it on in the settings, an AI client on **one PC you specify** (or a narrow subnet) can connect over your network. Every request needs an access token, and Windows Firewall lets in only that address. Turning remote use off closes the port.

## What Marionette stores on your PC

All of it stays on your PC; uninstalling removes the app's files (see each edition below).

- Settings (language, input mode, models, remote-use state).
- App notes: tips about apps Marionette has operated (app names, window titles, short notes, and short summaries of recent tool calls attached as evidence).
- Logs of the server's activity (tool names, timings and errors) for troubleshooting.
- The Free edition's hourly usage count, and a license key if you entered one. These two files are encrypted with Windows DPAPI.

## Internet access

Marionette itself sends nothing to the developer. It connects to the internet only for:

- **Microsoft Store edition:** license (Pro add-on) and update checks, handled by the Microsoft Store and Windows.
- **Direct edition:** a daily check for a new version on GitHub (`github.com/kumting1103/Marionette-releases`), which receives the usual request information (IP address, user agent with the Marionette version).

Your AI client and its AI service are separate products with their own network use and policies.

## Children

Marionette is a developer tool and is not directed to children under 13.

## Changes

If this policy changes, the new version is posted at this address with a new effective date. Earlier versions are kept in the page's history.

## Contact

Questions about this policy: kumting1103@gmail.com

---

# 개인정보 처리방침 {#ko}

시행일: 2026-10-26 · 개발자: 오세웅(RadishCode Labs) · 연락처: kumting1103@gmail.com

Marionette MCP(이하 "Marionette")는 사용자가 실행하는 AI 클라이언트(예: Claude Code)가 Model Context Protocol(MCP)로 이 PC의 화면을 보고 데스크톱 앱을 조작하게 해 주는 Windows 앱입니다. 이 방침은 Marionette가 PC 안의 정보를 어떻게 다루는지 설명합니다.

## 요약

- Marionette에는 **계정, 분석, 원격 측정(텔레메트리)이 없습니다.** 개발자는 사용자의 화면, 글자, 파일, 사용 내역을 받지 않습니다.
- 화면 캡처, 글자 인식(OCR), 화면 분석은 **사용자의 PC 안에서** 합니다.
- 결과는 **사용자가 Marionette에 연결한 AI 클라이언트로만** 보냅니다. 그 뒤의 처리는 그 클라이언트와 AI 서비스의 정책을 따릅니다.

## Marionette가 다루는 정보

| 정보 | 처리 |
| --- | --- |
| 화면 내용(화면·창·영역의 캡처) | AI 클라이언트가 도구를 부를 때 캡처합니다. PC 안에서 분석하고(글자 인식, 아이콘 탐지, Windows UI Automation 이름), 현재 세션 동안 메모리에만 두며 디스크에 쓰지 않습니다. |
| 인식한 글자, 요소 목록, 창 제목, 앱 이름 | 도구 결과로 연결된 AI 클라이언트에 돌려줍니다. |
| 스크린샷 | AI 클라이언트가 이미지를 요청할 때만 돌려줍니다. |
| AI 클라이언트가 입력하는 글자 | 대상 앱에 키보드 입력으로 보냅니다. 한글 등 일부 글자는 클립보드에 잠깐 넣어 붙여 넣은 뒤, 원래 있던 클립보드 글자로 되돌립니다. |
| 사용자의 키보드 입력 | **기록하지 않습니다.** 긴급 정지용 단축키 하나(기본 Ctrl+Alt+Q)만 등록하고 다른 키는 기록하지 않습니다. |

## 결과가 가는 곳

- **이 PC에서 사용(기본)**: AI 클라이언트는 `127.0.0.1`로 Marionette에 연결합니다(이 PC의 프로그램만 접속 가능). 결과는 AI 클라이언트가 자기 AI 서비스로 보내기 전까지 PC 안에 있고, 그 뒤에는 그 서비스의 개인정보 처리방침(Claude Code라면 Anthropic)을 따릅니다.
- **원격 사용(기본 꺼짐)**: 설정에서 켜면 **사용자가 지정한 PC 한 대**(또는 좁은 서브넷)의 AI 클라이언트가 네트워크로 연결할 수 있습니다. 모든 요청에 접속 토큰이 필요하고, Windows 방화벽은 그 주소만 들여보냅니다. 끄면 포트를 닫습니다.

## PC에 저장하는 것

모두 사용자의 PC에만 저장합니다. 제거하면 앱 파일이 지워집니다(판별 아래 참고).

- 설정(언어, 입력 방식, 모델, 원격 사용 상태)
- 앱 노트: Marionette가 다뤄 본 앱의 요령(앱 이름, 창 제목, 짧은 노트, 근거로 붙는 최근 도구 호출의 짧은 요약)
- 문제 해결용 서버 동작 로그(도구 이름, 시간, 오류)
- Free판의 시간당 사용 횟수, 입력한 라이선스 키. 이 두 파일은 Windows DPAPI로 암호화합니다.

## 인터넷 접속

Marionette는 개발자에게 아무것도 보내지 않습니다. 인터넷에는 다음 경우에만 접속합니다.

- **Microsoft Store판**: 라이선스(Pro 추가 기능)와 업데이트 확인. Microsoft Store와 Windows가 처리합니다.
- **직접 계약판**: 하루 한 번 GitHub(`github.com/kumting1103/Marionette-releases`)에서 새 버전 확인. 일반적인 요청 정보(IP 주소, Marionette 버전이 담긴 사용자 에이전트)가 전달됩니다.

AI 클라이언트와 AI 서비스는 별개의 제품으로, 각자의 네트워크 사용과 정책이 있습니다.

## 아동

Marionette는 개발자 도구이며 13세 미만 아동을 대상으로 하지 않습니다.

## 변경

방침이 바뀌면 새 시행일과 함께 이 주소에 게시합니다. 이전 판은 페이지 기록에 남습니다.

## 연락처

이 방침에 대한 문의: kumting1103@gmail.com
