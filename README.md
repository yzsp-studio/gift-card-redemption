<div align="center">

# 🎬 gift-card-redemption

## 先 PREPARE 查清套餐，另起一条消息确认才 REDEEM
## PREPARE checks the plan; a separate reply unlocks REDEEM

📮 **商务合作 / Business：wow.vip@foxmail.com**
🎬 **抖音 / Douyin：[v.douyin.com/07EjIDGVErY](https://v.douyin.com/07EjIDGVErY/)**

</div>

---

## 🇨🇳 中文

查询订阅礼品卡的可兑换状态和套餐，并在确认后完成兑换。支持文本兑换码和上传的二维码图片，图片只使用当前对话中实际上传附件对应的运行时地址并原样传递，不构造、不改写。PREPARE 是只读查询，返回确认信息与兑换令牌；只有当确认信息已展示、当前回复已结束、用户在后续新消息中明确同意，且该消息没有提交新码或新图时，才会调用一次 REDEEM。不可兑换、工具异常或返回结构不完整时立即停止，不进入兑换。不处理购买、退款、订单、优惠券或其他来源的礼品卡。

### ✨ 能做什么

- 输入文本兑换码或二维码图片 → PREPARE 返回可兑换状态与目标套餐，不执行兑换
- 展示套餐、目标账号、生效说明与兑换规则后结束回复，等待独立确认回合
- 新消息明确同意才调用一次 REDEEM，兑换令牌原样传递，不解析、不修改、不展示
- 同一条消息里的确认、预先授权、询问、犹豫、拒绝或取消均不触发兑换
- 提交新码或新图即清除待确认状态并重新走 PREPARE，不沿用旧结果
- 只传兑换码或图片地址等业务参数，不传账号标识、凭据或其他运行时上下文

### 📦 包含的技能

- `gift-card-redemption` —— 见 [`gift-card-redemption/SKILL.md`](gift-card-redemption/SKILL.md)

### 🚀 安装

```bash
git clone https://github.com/yzsp-studio/gift-card-redemption.git
cp -r gift-card-redemption/* "$DSH_HOME/skills/"
```

> 技能是**纯文本说明**（`SKILL.md` + `references/`），零依赖、零 API key，用你当前 agent 的会话额度。

---

## 🇬🇧 English

Queries the redemption status and packages of subscription gift cards, then completes the redemption after confirmation. It accepts a typed redemption code or an uploaded QR-code image; an image uses only the runtime URL of the attachment actually uploaded in the current conversation, passed through verbatim and never constructed or rewritten. PREPARE is a read-only check that returns confirmation details plus a redemption token; REDEEM runs once only after those details were shown, the reply ended, the user explicitly agreed in a later message, and that message carried no new code or image. Unredeemable codes, tool errors, or incomplete responses stop the flow immediately. It does not handle purchases, refunds, orders, coupons, or gift cards from other sources.

### ✨ What it does

- A typed code or QR image in, PREPARE out: redeemable status and target package, with no redemption performed
- Shows package, target account, effective terms, and rules, then ends the reply to wait for a standalone confirmation turn
- Only an explicitly agreeing new message triggers one REDEEM; the token is passed verbatim and never parsed, altered, or displayed
- Same-message confirmations, pre-authorization, questions, hesitation, refusal, or cancellation never trigger a redemption
- Submitting a new code or image clears the pending state and returns to PREPARE instead of reusing old results
- Sends business parameters only — code or image URL — never account identifiers, credentials, or other runtime context

### 📦 Skills included

- `gift-card-redemption` — [`gift-card-redemption/SKILL.md`](gift-card-redemption/SKILL.md)

### 🚀 Install

```bash
git clone https://github.com/yzsp-studio/gift-card-redemption.git
cp -r gift-card-redemption/* "$DSH_HOME/skills/"
```

> Skills are **plain-text instructions** (`SKILL.md` + `references/`). Zero dependencies, no API keys — they run on your agent's existing session quota.

---

## 📮 联系 / Contact

| | |
|---|---|
| 🎬 **抖音 / Douyin** | [https://v.douyin.com/07EjIDGVErY/](https://v.douyin.com/07EjIDGVErY/) |
| 📮 **商务合作 / Business** | **wow.vip@foxmail.com** |
| 🐙 **GitHub** | [https://github.com/yzsp-ai](https://github.com/yzsp-ai) |
| 💖 **打赏 / Support** | [afdian.com/a/yzsp-ai](https://afdian.com/a/yzsp-ai) |

## 📄 License

[MIT](LICENSE) · © 2026 [yzsp-ai](https://github.com/yzsp-ai)
