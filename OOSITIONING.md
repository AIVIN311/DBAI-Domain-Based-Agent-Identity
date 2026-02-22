# DBAI Positioning — Identity Discovery as Glue Layer

DBAI 並非一個新的完整身份系統，而是一個 **identity discovery convention**，
其角色是連接現有身份模型，而非取代它們。

---

## 1. The Identity Stack Context

在數位與 agent 生態中，身份可粗略分為三層：

| Layer | Problem | Typical Systems |
|------|---------|-----------------|
| Naming / Anchor | Actor 如何被持久識別與發現 | DNS, ENS, platform IDs |
| Control / Proof | 誰控制這個 actor | DID, PKI, wallet keys |
| Capability / Action | Actor 能做什麼 | OAuth, tokens, policy engines |

DBAI 位於：
> **Naming / Anchor 與 Control / Proof 的交界**

也就是：
- 提供 actor discoverability
- 綁定 anchor 與 controller
- 不定義 capability

---

## 2. Relationship with DID

DID 提供：
- 密鑰控制
- 可驗證身份
- 憑證發行能力

DBAI 提供：
- discoverability root
- anchor persistence
- context binding

關係：
- DID 可以作為 DBAI `controllers`
- DBAI 可讓 DID identity 更易被發現
- DBAI 不定義 DID method

👉 DBAI = discoverability  
👉 DID = control semantics

---

## 3. Relationship with Wallet Identity

Wallet identity 提供：
- 經濟能力
- transaction signing
- delegation

限制：
- address 可變
- 多鏈碎片化
- 語境較弱

DBAI 與 wallet 的關係：
- wallet 可作為 controller 或 capability container
- DBAI 提供 wallet 與 actor 的語境連結
- DBAI 不定義經濟或 capability 模型

👉 Wallet = capability  
👉 DBAI = persistent reference

---

## 4. Relationship with DNS and Naming Systems

DBAI 採用 DNS 作為初始 anchor，因為：
- 全球唯一 namespace
- 廣泛部署
- 社會與制度語境

但 DBAI：
- 不改變 DNS 協議
- 不取代其他 naming systems
- 不排除未來其他 anchor 形式

DNS 是 deployment substrate，而非 DBAI 的權威來源。

---

## 5. Relationship with Platform Identity

平台身份（帳號）提供：
- 易用性
- 內建信任網路
- runtime context

但平台身份通常：
- 封閉
- 不可攜
- 不具持久 discoverability

DBAI 提供：
- 平台外 identity anchor
- 跨平台 actor reference
- 去中心 discoverability

👉 Platform ID = context-bound identity  
👉 DBAI = context-independent identity anchor

---

## 6. Relationship with Indexes and Discovery Graphs

DBAI 定義 resolver，但不定義 index。

預期生態：
- Resolver 提供 existence lookup
- Index 提供 search / ranking / graph

這與 DNS 與搜尋引擎的關係類似。

DBAI 的立場：
- identity 不應依賴 index 存在
- index 應為可競爭與可替代層

---

## 7. DBAI as Glue Layer

DBAI 的核心角色是：
- 連接 naming 與 control
- 連接 domain 與 DID / wallet
- 連接 actor 與 runtime
- 提供 identity rendezvous point

DBAI 不競爭：
- SSI frameworks
- Credential ecosystems
- Capability models
- Reputation systems

👉 DBAI 讓不同 identity 系統可以「找到彼此」。

---

## 8. Why This Layer Matters

在 agentic web 中，缺少 persistent identity anchor 會導致：
- actor identity fragmentation
- trust accumulation 困難
- governance 邊界模糊
- 跨平台協作成本增加

DBAI 提供的不是完整解決方案，而是：
> 一個讓其他身份模型能互相對齊的最小地板

---

## 9. Long-Term View

如果 DID 提供密鑰語言，  
如果 wallet 提供經濟語言，  
如果 capability 提供行動語言，  

那 DBAI 嘗試提供：
> actor existence 的語言

這使 actor identity 更接近 URL，而非帳號。