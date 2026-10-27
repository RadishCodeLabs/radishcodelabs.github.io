---
title: Marionette MCP — Privacy Policy
---

# Marionette MCP — Privacy Policy

Effective date: 2026-10-26 · Developer: Sewoong Oh (RadishCode Labs) · Contact: kumting1103@gmail.com

[한국어](ko/privacy)

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
| Your own keyboard input | **Not recorded.** Marionette registers one global hotkey (the emergency stop, Ctrl+Alt+Backspace by default) and does not log other keys. |

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
