# DBAI FAQ — Domain-Based Agent Identity

這份 FAQ 用於釐清 DBAI 的定位、範圍與常見誤解。  
DBAI 是一個 **identity discovery convention**，而非完整身份系統。

---

## ❓ DBAI 是什麼？

DBAI 定義一種以 DNS 網域為錨點的 Agent 身分發現方式，使不同平台與 runtime 能解析同一 actor 的持久 identity。

DBAI 提供：
- Anchor-based persistence
- Manifest discovery
- Control proof binding

DBAI 不提供：
- Credential 語義
- Reputation
- Capability taxonomy
- Runtime attestation

---

## ❓ DBAI 是不是另一個 DID？

不是。

DID 解決的是 **控制與可驗證身份**；  
DBAI 解決的是 **可解析與持久錨點**。

兩者關係：
- DID 可以作為 DBAI `controllers`
- DBAI 可以作為 DID 的 discoverability root

DBAI 與 DID 是互補，而非競爭。

---

## ❓ 為什麼不用 Wallet Address 當 Anchor？

Wallet address：
- 可變（多鏈 / 多帳戶）
- 缺乏語境（組織 / 法域）
- discoverability 弱

Domain 提供：
- 全球唯一 namespace
- 長期持久性
- 社會與制度語境
- 既有解析基礎設施

Wallet 更適合作為 capability / economic identity，而非 anchor。

---

## ❓ DBAI 是否取代 DNS、ENS 或其他命名系統？

不是。

DBAI 只是一種「如何用 namespace 作為 identity anchor」的約定。  
DNS 是目前最廣泛部署的 namespace，但 DBAI 不排除未來其他 anchor 形式。

---

## ❓ DBAI 需要中心化 registry 嗎？

不需要。

- Namespace authority 來自 domain 控制
- Resolver 可多實作
- Extension schema 無需註冊
- Index 可自然長出但不影響 identity validity

DBAI 的設計目標是 **去中心 discoverability**。

---

## ❓ 為什麼 DBAI 不定義 agent 類型或能力？

因為 identity 與語義分離可以確保：
- 長期穩定性
- 跨 paradigm 演化
- 避免標準戰爭

語義、能力與聲譽應在 extension 或上層協議定義。

---

## ❓ Extension schema 是否是標準的一部分？

不是。

Schema 只是 **informational hint**，幫助 index 或 consumer 理解 extension。  
Resolver 不必抓 schema 即可驗證 identity。

---

## ❓ DBAI 是否會有 Index 或 Discovery Graph？

可能，但 DBAI 不定義 index。

DBAI 預期：
- Resolver 提供存在解析
- Index 提供可見性與搜尋

這種分離與 DNS + 搜尋引擎的關係類似。

---

## ❓ DBAI 是否與 AI Agent 綁定？

DBAI 可以用於：
- AI agent
- Bot
- 自動化服務
- 數位分身
- 組織服務

DBAI 定義 actor identity，而非 AI 專屬身份。

---

## ❓ DBAI 的長期目標是什麼？

長期目標是提供一個：
- 中立
- 持久
- 去中心
- 可互通

的 actor identity discovery 層，使 AI 與數位 actor 能像網站一樣被解析與存在。

DBAI 希望成為地板，而不是完整身份系統。