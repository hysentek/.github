<div align="center">

# Hysentek

**Agent infrastructure for DeepSeek Harness — built in the open, shipped every day.**

![repos](https://img.shields.io/badge/repositories-7-0b7285?style=flat-square)
![commits today](https://img.shields.io/badge/2026--11--23-24%20commits-2f9e44?style=flat-square)
![products](https://img.shields.io/badge/products%20advanced-3-1c7ed6?style=flat-square)
![blockers](https://img.shields.io/badge/blockers-0-868e96?style=flat-square)

<sub>Daily engineering report · Monday, 23 November 2026 · Asia/Saigon · snapshot 15:33</sub>

</div>

---

## 📊 Today at a glance

| Metric | Today |
|:--|--:|
| Repositories with commits | **5 / 7** |
| Commits | **24** |
| Files changed | **235** |
| Lines added | **≈ 34.8k** |
| Products advanced | **3** |
| Blockers | **0** |

Three product tracks moved forward in one day: the **Agent Bus** platform, its
**DeepSeek Harness bridge**, and the **Stage Show** live-theater plugin.

---

## 🕐 The day, hour by hour

| Time (UTC+7) | Milestone |
|:--|:--|
| 10:46 | Agent Bus — architecture spec and project skeleton published |
| 11:40 | Agent Bus — worker API, durable-object bus, D1 schema, React ops dashboard and tests implemented end to end |
| 11:44 | Agent Bus — organisation email onboarding with real OTP delivery |
| 12:28 | Agent Bus — agent email service: HTML send, inbound capture, inbox API |
| 12:32 | Agent Bus — shared-key bootstrap, public onboarding docs, footer links |
| 13:21 | DSH bridge — first working plugin: sessions as bus addresses |
| 13:28 | DSH bridge — WebSocket-first transport, long-poll fallback, failover verified against production |
| 13:37 | DSH bridge — zero-config self-registration for new agents |
| 13:38 | Welcome — onboarding README refreshed |
| 14:33 | DSH bridge — agent working protocol (EN + VI) and milestone announcements |
| 14:43 | Org profile — this page published |
| 14:54 | DSH bridge — repository-as-source-of-truth status policy and task acknowledgement |
| 15:01 | Stage Show — cross-session live theater with automatic replay |
| 15:21 | Welcome — final README pass |

---

## 🏗️ What we are building

### 1 · Hysen Agent Bus

> A central nervous system for internal AI agents.

A communication network that lets agents address each other, hand off work and
exchange mail: edge worker API, durable-object bus, D1 persistence, a React
operations dashboard, and an agent mail service — with onboarding documents and
a test suite.

**Today:** first complete implementation, live agent email delivery on the
`hyratek.ai` domain, shared-key zero-config bootstrap, and public onboarding docs.

---

### 2 · Hysen Agent Bus → DeepSeek Harness bridge

> Every agent gets an address; every inbound message becomes a Session task.

The DSH plugin that connects a harness agent to the bus: inbound work lands as a
Session notice, replies return to the sender automatically, and long-running work
never blocks delivery.

**Today:** WebSocket-first transport with long-poll fallback (failover verified
against the production deployment), zero-config self-registration, agent name and
address in the install flow, a bilingual working protocol, and the milestone
`notify` tool.

---

### 3 · DSH Stage Show

> Live AI engineering theater, straight from the conversation.

A DSH Web plugin that turns a session into a full-screen command center: the
running session appears live, idle time replays the newest history, and every
tool call, terminal output, diff and timeline event is rendered as it happens —
with recordings you can seek, step and speed up.

**Today:** first build with cross-session live theater and automatic replay.

---

## 🧩 Supporting work

| Workstream | What changed |
|:--|:--|
| **Welcome** | Onboarding README tightened to the exact toolchain an engineer needs to start |
| **Org profile** | `hysentek/.github` created; this page is now the org's public front door |
| **Onboard** | Repository created and reserved for the upcoming guided onboarding flow |
| **Hysen DSH branding** | White-label identity for the harness Web app (published) |

---

## 📈 By the numbers

| Repository | Focus | Commits | Files | Lines |
|:--|:--|--:|--:|--:|
| `hyra-agent-bus` | Agent Bus platform (API, dashboard, mail) | 8 | 128 | +13.4k |
| `hysen-agent-bus-dhs-plugin` | Harness bridge and agent protocol | 10 | 81 | +7.5k |
| `dsh-stage-show` | Live theater plugin for DSH Web | 1 | 21 | +13.9k |
| `Welcome` | Onboarding guide | 3 | 3 | +13 |
| `.github` | Org profile | 2 | 2 | +13 |
| `onboard` | Scaffolded, no code yet | 0 | 0 | — |
| **Total** | | **24** | **235** | **+34.8k** |

<sub>Figures are a snapshot at 15:33 UTC+7 on 23 November 2026 and exclude this report's own publishing and metadata commits.</sub>

---

## 🇻🇳 Tóm tắt cho lãnh đạo

- **Agent Bus đã chạy được đầu–cuối**: API worker, bus Durable Object, D1, dashboard
  React, và dịch vụ email cho agent — đã gửi OTP thật trên `hyratek.ai`.
- **Cầu nối sang DeepSeek Harness**: mỗi agent có địa chỉ riêng, nhận việc tự động
  qua Session, trả lời tự động; transport WebSocket là chính, long-poll dự phòng,
  đã kiểm tra failover trên môi trường production.
- **Cài đặt không cần cấu hình**: agent mới tự đăng ký bằng shared key, tên và địa
  chỉ nằm ngay trong prompt cài đặt.
- **Stage Show**: plugin "sân khấu" live cho DSH Web, theo dõi session đang chạy,
  tự replay khi rảnh, ghi và tua lại phiên làm việc.
- **Không có blocker**; toàn bộ thay đổi đã nằm trên `main` của từng repo.

---

<div align="center">

**Public repositories** · [`.github`](https://github.com/hysentek/.github) · [`hysen-dsh-branding`](https://github.com/hysentek/hysen-dsh-branding)

<sub>Report generated from repository activity on 23 November 2026, 00:00–24:00 (UTC+7).</sub>

</div>
