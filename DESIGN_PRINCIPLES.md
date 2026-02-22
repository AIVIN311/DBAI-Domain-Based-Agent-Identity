# DBAI Design Principles

DBAI 的設計目標不是定義 agent identity 的全部，而是提供一個
**persistent, neutral, discoverable anchor**。

---

## 1. Identity-Only Core
DBAI 只解決：
- Actor 如何被識別
- Actor 如何被發現
- Actor 如何證明 anchor 控制關係

DBAI 不解決：
- Actor 做什麼
- Actor 是否可信
- Actor 有哪些能力

---

## 2. Anchor-Based Persistence
Domain 作為 anchor 提供：
- 長期可解析性
- 社會與制度語境
- 去中心 namespace

Anchor ≠ authority  
Anchor 是 rendezvous point。

---

## 3. Resolver Decentralization
Resolver 是行為，不是服務：
- 多實作
- 本地可驗證
- 不依賴中心 API

這確保 actor existence 不受單一 gateway 控制。

---

## 4. Semantic Separation
Identity 與語義分離：
- Extensions 為 opaque
- Schema 為 informational
- Index 與 capability 為外部層

這確保 identity 能跨 paradigm 演化。

---

## 5. Domain-Based Namespace
Extension namespace 使用 domain-based URI：
- 去中心唯一性
- 語義權威由 namespace domain 控制
- 與 DBAI anchor 拓撲對齊

---

## 6. Emergent Ecosystem
DBAI 預期：
- Index 會自然長出
- Semantic patterns 會形成
- Governance 會演化

DBAI 提供地板，而非天花板。

---

## 7. Minimal Spec, Maximum Surface
DBAI 偏好：
- 小而清晰的 core
- 可擴展邊界
- 低 adoption friction

基礎設施的成功來自不可見的穩定，而非功能豐富。# DBAI Design Principles

DBAI 的設計目標不是定義 agent identity 的全部，而是提供一個
**persistent, neutral, discoverable anchor**。

---

## 1. Identity-Only Core
DBAI 只解決：
- Actor 如何被識別
- Actor 如何被發現
- Actor 如何證明 anchor 控制關係

DBAI 不解決：
- Actor 做什麼
- Actor 是否可信
- Actor 有哪些能力

---

## 2. Anchor-Based Persistence
Domain 作為 anchor 提供：
- 長期可解析性
- 社會與制度語境
- 去中心 namespace

Anchor ≠ authority  
Anchor 是 rendezvous point。

---

## 3. Resolver Decentralization
Resolver 是行為，不是服務：
- 多實作
- 本地可驗證
- 不依賴中心 API

這確保 actor existence 不受單一 gateway 控制。

---

## 4. Semantic Separation
Identity 與語義分離：
- Extensions 為 opaque
- Schema 為 informational
- Index 與 capability 為外部層

這確保 identity 能跨 paradigm 演化。

---

## 5. Domain-Based Namespace
Extension namespace 使用 domain-based URI：
- 去中心唯一性
- 語義權威由 namespace domain 控制
- 與 DBAI anchor 拓撲對齊

---

## 6. Emergent Ecosystem
DBAI 預期：
- Index 會自然長出
- Semantic patterns 會形成
- Governance 會演化

DBAI 提供地板，而非天花板。

---

## 7. Minimal Spec, Maximum Surface
DBAI 偏好：
- 小而清晰的 core
- 可擴展邊界
- 低 adoption friction

基礎設施的成功來自不可見的穩定，而非功能豐富。