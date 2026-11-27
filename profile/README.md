<div align="center">

# Hysentek

**Agent infrastructure for DeepSeek Harness — built in the open, shipped every day.**

![repos](https://img.shields.io/badge/repositories-7-0b7285?style=flat-square)
![issues](https://img.shields.io/badge/HysenGeo-43%2F44%20issues-2f9e44?style=flat-square)
![products](https://img.shields.io/badge/product%20tracks-4-1c7ed6?style=flat-square)
![blockers](https://img.shields.io/badge/blockers-2-c92a2a?style=flat-square)

<sub>Engineering snapshot · Friday, 27 November 2026 · Asia/Saigon · snapshot 14:00</sub>

</div>

---

## 📊 Today at a glance

| Metric | Snapshot |
|:--|--:|
| Active product tracks | **4** |
| HysenGeo issues closed | **43 / 44** |
| HysenGeo gates closed | **5 / 6** (M0, P0, P1, P2, P3) |
| Blockers | **2** (GitHub Actions billing; owner approvals for the real pilot) |

Four product tracks are moving: **HysenGeo**, the **Agent Bus** platform, its
**DeepSeek Harness bridge**, and the **Stage Show** live-theater plugin.

---

## 🕐 Recent milestones

| Time (UTC+7) | Milestone |
|:--|:--|
| 11:24 | HysenGeo — P1 gate closed: five sensors, deterministic diagnosis, source map, GEO Index, baseline pipeline |
| 12:00 | HysenGeo — P2 gate closed: 11-rule policy guard, policy-filtered planner, automatic plan PRs, append-only approvals |
| 13:38 | HysenGeo — P3 gate closed: idempotent executor, DroidPilot and browser adapters, verifier, end-to-end chaos demo |
| 13:52 | HysenGeo — pilot report with difference-in-differences, provenance for every figure, recorded-data warning |
| 13:58 | Bus plugin 0.2.6 — manual task rows now carry their workspace; cancel of an unknown job returns 404; self-messages no longer open a Turn |
| 14:00 | HysenGeo — 43 of 44 issues closed; final gate remaining |

---

## 🏗️ What we are building

### 1 · HysenGeo

> Generative Engine Optimization for Vietnamese businesses — measured, not promised.

An end-to-end system that measures how a brand appears in AI answers
(ChatGPT, Perplexity, Google AI Mode, Gemini, Copilot), diagnoses why it is
missing or misrepresented, and turns that into policy-guarded work: every fact
needs a source, every published action needs a human approval, every executed
action is verified and cited back to evidence.

**Status (27 Nov):** **43 of 44 issues closed**, five of six gates passed
(specification, data, measurement, governance, execution). Working today:
multi-engine sensors within ToS limits, deterministic claim matching and source
mapping, the GEO Index with bootstrap confidence intervals, an 11-rule policy
guard with ablation tests, a planner that drops policy-violating actions, automatic
plan pull requests, an append-only approval flow, idempotent execution through
DroidPilot and browser adapters, verification with content hashes, control-group
difference-in-differences, and a client pilot report with per-figure provenance.

**Not yet:** a real-data pilot. Every number so far is fake/recorded and the
reports say so; running the real baseline needs owner-approved prompt sets,
API keys and posting accounts.

---

### 2 · Hysen Agent Bus

> A central nervous system for internal AI agents.

A communication network that lets agents address each other, hand off work and
exchange mail: edge worker API, durable-object bus, D1 persistence, a React
operations dashboard, and an agent mail service — with onboarding documents and
a test suite.

**Today:** first complete implementation, live agent email delivery on the
`hyratek.ai` domain, shared-key zero-config bootstrap, and public onboarding docs.

---

### 3 · Hysen Agent Bus → DeepSeek Harness bridge

> Every agent gets an address; every inbound message becomes a Session task.

The DSH plugin that connects a harness agent to the bus: inbound work lands as a
Session notice, replies return to the sender automatically, and long-running work
never blocks delivery.

**Today:** WebSocket-first transport with long-poll fallback (failover verified
against the production deployment), zero-config self-registration, agent name and
address in the install flow, a bilingual working protocol, and the milestone
`notify` tool.

---

### 4 · DSH Stage Show

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

## 🏢 Fleet — 26 November 2026

| Host | Agent | Bus identity | Status repository |
|:--|:--|:--|:--|
| `macom00` | MarCom 00 | `macom@hyratek.ai` | `hysentek/marcom` (internal) |

MarCom 00 runs the harness bridge at generation `45c44fe` — hash-verified file by file
against upstream — and stays connected to the bus over WebSocket. Install evidence,
incidents and hand-offs live in that repository's `docs/status.md`; this page keeps the
one-paragraph summary.

---

## 🇻🇳 Tóm tắt cho lãnh đạo

- **HysenGeo — sản phẩm GEO cho doanh nghiệp Việt đã xong 43/44 issue, 5/6 gate GO.**
  Đo được thương hiệu trong câu trả lời AI (ChatGPT, Perplexity, Google AI Mode,
  Gemini, Copilot), chẩn đoán vì sao thiếu/sai, rồi lập kế hoạch hành động có luật
  bảo vệ: mọi dữ kiện phải có nguồn, mọi bài đăng phải có người duyệt, mọi action
  đã chạy phải được xác minh và trỏ bằng chứng.
- **Chưa chốt số thật**: toàn bộ số hiện tại là fake/recorded, báo cáo ghi rõ không
  dùng để công bố. Muốn chạy pilot thật cần sếp duyệt: bộ prompt mẫu (#15 + ngành #2),
  số liệu kinh doanh (#8), cấp key (Perplexity/Gemini) và tài khoản đăng bài.
- **Agent Bus đã chạy đầu–cuối**: API worker, bus Durable Object, D1, dashboard React,
  email agent thật trên `hyratek.ai`; cầu nối DeepSeek Harness cho mỗi agent một địa
  chỉ, nhận việc tự động qua Session, WebSocket là chính và long-poll dự phòng.
- **Stage Show**: plugin "sân khấu" live cho DSH Web, tự replay khi rảnh, ghi và tua
  lại phiên làm việc.
- **2 blocker**: (1) **GitHub Actions bị billing** — CI không chạy, kỹ thuật đang bù
  bằng gate local đầy đủ trước mỗi merge; (2) **owner chưa duyệt** bộ prompt và số
  liệu để chạy pilot thật.
- **(26/11) MarCom 00**: agent MarCom trên `macom00` đã nối bus (WebSocket), bridge
  generation `45c44fe` xác minh hash từng file; trạng thái ghi tại `hysentek/marcom`.

---

<div align="center">

**Public repositories** · [`.github`](https://github.com/hysentek/.github) · [`hysen-dsh-branding`](https://github.com/hysentek/hysen-dsh-branding)

<sub>Snapshot of repository state on 27 November 2026, 14:00 UTC+7. Details live in each repository's docs/status.md.</sub>

</div>
