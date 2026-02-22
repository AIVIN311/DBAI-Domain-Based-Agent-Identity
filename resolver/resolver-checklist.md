# DBAI Resolver Checklist (v0.1)

## Inputs
- Expected anchor domain (e.g., `algorithmicallocation.systems`)
- Agent identifier (preferred: `agent.<anchor-domain>`)

## Steps (MUST)
1) **Resolve endpoint**
   - Build manifest URL:
     - `https://agent.<anchor>/.well-known/agent-manifest.json`
     - fallback: `https://<anchor>/.well-known/agent-manifest.json`

2) **Fetch manifest over HTTPS**
   - Follow redirects cautiously (log final URL)

3) **Verify signature (`proof`)**
   - Determine verification method from `proof`
   - Verify that manifest bytes match signed payload

4) **Validate anchor consistency**
   - Ensure `manifest.anchor` equals expected anchor
   - Ensure `manifest.id` is consistent with the agent domain/URL context (policy choice)

5) **Process core fields**
   - `controllers`, `endpoints`, `keys` usable for downstream binding

## Rules (MUST NOT)
- MUST NOT require extension schema retrieval to consider identity valid
- MUST treat unknown `extensions` namespaces as opaque

## Optional hardening (SHOULD)
- Cache with short TTL
- Support revocation pointers under `revocations`
- DNSSEC validation / registry-lock signals (ops/policy)