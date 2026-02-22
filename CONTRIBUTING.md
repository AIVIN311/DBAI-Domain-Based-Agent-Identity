# Contributing to DBAI

DBAI 採取 **minimal core, open edge** 的設計哲學。  
貢獻應優先維持 identity 核心穩定，並將創新放在 extension 或 guidance 層。

---

## Ways to Contribute

### 1. Spec Clarification
- 編輯錯字
- 改善語意
- 增加非規範性說明

### 2. Resolver Guidance
- 提供實作經驗
- 補充驗證流程
- 分享快取或操作建議

### 3. Extension Patterns
- 提供 domain-based namespace 範例
- 提供 schema（informational）
- 分享語義設計經驗

### 4. Ecosystem Notes
- Indexer 實驗
- Agent lifecycle 經驗
- Governance / policy 觀察

---

## Design Guardrails

貢獻 SHOULD：
- 保持 core minimal
- 避免 capability taxonomy
- 避免 credential 語義綁定
- 使用 domain-based namespace

貢獻 SHOULD NOT：
- 將 DBAI 轉為完整 SSI
- 引入中心化 registry 依賴
- 讓 extensions 影響 identity validity

---

## Proposing Extensions

Extension proposal 建議包含：
- Namespace（domain-based URI）
- Informational schema URL
- 使用情境說明
- 與 DBAI core 的分離說明

Extension 不需要 DBAI maintainer 批准即可存在；  
DBAI 僅記錄與整理 emergent patterns。

---

## Governance
目前為 maintainer-driven + open discussion。  
未來若社群成長，可演化為：
- lightweight working group
- community calls