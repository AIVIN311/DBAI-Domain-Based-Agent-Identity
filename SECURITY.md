# Security Policy — DBAI

DBAI 是一個 identity discovery convention，其安全性依賴：
- Anchor domain 的營運安全
- Manifest proof 的密鑰管理
- Resolver 的驗證正確性

DBAI 本身不定義 runtime、capability 或 credential 安全模型。

---

## Threat Model (Non-exhaustive)

### 1. Domain Hijack
攻擊者取得 registrar 帳戶或 DNS 控制權，發布惡意 manifest。

**Mitigations (Operational, recommended):**
- Registrar MFA
- Registry lock（若可用）
- 最小權限 DNS 操作
- DNSSEC（optional but recommended）

---

### 2. Manifest Tampering / MITM
攔截或改寫 manifest 內容。

**Mitigations:**
- HTTPS
- Manifest proof（JWS/COSE）
- Short cache TTL

---

### 3. Key Compromise
控制者密鑰外洩，導致惡意簽章。

**Mitigations:**
- Key rotation
- Revocation pointers
- Hardware-backed keys（optional）

---

### 4. Extension Confusion
惡意或誤導性的 extension namespace 或 schema。

**Mitigations:**
- Domain-based namespace authority
- Resolver treating extensions as opaque
- Consumers performing independent validation

---

## Out of Scope
- Capability misuse
- Runtime sandbox escape
- Reputation manipulation
- Index ranking manipulation

---

## Vulnerability Disclosure
若發現可能影響 DBAI 規範或示例實作的安全問題，請：
1. 提 issue（標記 `security`）
2. 或私下聯絡 maintainer

DBAI 目前為 pre-standard project，建議負責任揭露。