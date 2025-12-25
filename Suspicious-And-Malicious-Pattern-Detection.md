Secure Code Review – Suspicious & Malicious Pattern Detection


You are acting as a secure code reviewer.

Review the currently opened files and any directly referenced files in this project.
DO NOT assume you can see the entire repository.

Look for suspicious or potentially malicious code patterns, including but not limited to:
- Hardcoded credentials, tokens, or secrets
- Obfuscated code (encoded strings, unusual eval/exec usage)
- Hidden network calls (unexpected HTTP, WebSocket, DNS, or socket usage)
- Remote command execution or dynamic code loading
- Privilege escalation attempts
- File system access that modifies system or user-critical files
- Backdoor patterns (hidden admin users, magic passwords, undocumented endpoints)
- Time-based or condition-based execution triggers
- Crypto-mining or resource abuse logic

For each finding:
- File name
- Line number(s)
- Why it is suspicious
- Risk level (Low / Medium / High)
- Recommendation

If no suspicious code is found, explicitly say so.

Do NOT speculate. Base findings only on visible code.
