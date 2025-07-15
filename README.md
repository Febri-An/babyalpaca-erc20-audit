# 🔍 Light Audit – ERC20 BabyAlpaca Token

**Auditor:** Febri Nirwana  
**Date:** July 2025  
**Contract Address:** `0xE7e93e0459FfDD8D6DcD4fF26Fc36D3682Cc6bFF`  
**Network:** Ethereum

## 📄 PDF Report
[👉 Download Full Audit Report](./BabyAlpaca_Audit_FebriNirwana_July2025.pdf)

## 🧠 Key Findings
- 🔴 Critical: Owner-controlled backdoor via `transferFrom()`
- 🟡 Medium: Unused `launch()` logic
- 🟢 Low: Dead code (`_transferAllowed()`, `exchanges`)

## ✅ Summary
This contract contains risky logic paths that could allow the owner to extract tokens before launch.  
It also avoids standard libraries like OpenZeppelin, introducing unnecessary complexity.

---

> Built and published by [@febrinirwana](https://github.com/febrinirwana)
