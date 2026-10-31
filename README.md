# kordef-owasp-llm-prompt-guard

> **Deterministic OWASP LLM Top 10 Input Guard & JWT/OAuth 2.0 Tool-Use Boundary Enforcer for Autonomous AI Agents**

Developed by **KOR DEF (Zero-Trust Cloud & AI Security Architecture)**.

---

## 🔒 Security Features

- **OWASP LLM01 Prompt Injection Guard**: Pre-inference input sanitizer enforcing structural boundary constraints to prevent direct and indirect prompt overrides.
- **OWASP LLM02 Sensitive Information Disclosure Shield**: Real-time regex and pattern guardrails for blocking PII, API tokens, and AWS credentials in model outputs.
- **OWASP LLM07 System Prompt Leakage Prevention**: Canonical prompt wrapper preventing system directive extraction.
- **Agent Tool-Use Boundary Enforcer**: OAuth 2.0 and JWT scoped validation preventing unauthorized function execution by autonomous AI agents.

---

## ⚡ Quick Start

```python
from kordef_guard import LLMPromptGuard, ToolBoundaryEnforcer

guard = LLMPromptGuard(strict_mode=True)
sanitized_input = guard.sanitize_input(user_prompt)

tool_enforcer = ToolBoundaryEnforcer(jwt_token=auth_header)
tool_enforcer.validate_action(requested_tool="database_query")
```

---

## 🛡️ About KOR DEF
**KOR DEF** specializes in AI security guardrails, zero-trust cloud architecture, and DevSecOps automation.
- **Website**: kordefence.net
- **Contact**: info@kordefence.com
