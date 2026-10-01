# Pink Agentic AI Payments

Pink Agentic AI Payments (by PinkWallet, early access) is the approval layer between AI agents and company money: plain-language rules, per-agent budgets and human approvals decide each payment before a single-use card or bank transfer is issued.

## Try it

- **Live sandbox**: https://agentic-sandbox.pinkwallet.com/ — create a free workspace (test credentials only, no money moves; production not yet available).
- **MCP endpoint**: `https://agentic-sandbox.pinkwallet.com/mcp` (Streamable HTTP, `Authorization: Bearer <agent key>`), 7 tools: `pink.get_budget`, `pink.list_payees`, `pink.list_rules`, `pink.check_policy`, `pink.request_payment`, `pink.get_credential`, `pink.report_receipt`. Claude Code: `claude mcp add --transport http pink https://agentic-sandbox.pinkwallet.com/mcp --header "Authorization: Bearer <AGENT_KEY>"`
- **Quickstart**: https://pinkwallet.com/agentic/developers/quickstart/ (full guides: https://pinkwallet.com/agentic/developers/) — listed in the official MCP Registry as `com.pinkwallet/agentic-payments-sandbox`.
- **Runnable examples**: https://github.com/Pink-Agentic-Payments/sandbox-examples (curl, Node MCP SDK, Python REST, an agent loop; MIT)

Try the interactive prototype (sample companies, no real money moves): https://claude.ai/public/artifacts/TpsUqLKnqZ3jHpghEGcimx

Status: early access. Join the waitlist for production access: https://pinkwallet.com/agentic/?utm_source=github&utm_medium=org-readme#early-access

## Open resources

- [agentic-payments-readiness](https://github.com/Pink-Agentic-Payments/agentic-payments-readiness): an open dataset scoring 16 payment providers on 7 agent-readiness dimensions, CC BY 4.0. · [Hugging Face](https://huggingface.co/datasets/Agentic-Payment/agentic-payments-readiness)
- [agent-spending-controls-crosswalk](https://github.com/Pink-Agentic-Payments/agent-spending-controls-crosswalk): a quoted crosswalk of how 14 payment providers and protocols let you cap AI agent spending, 43 rows, CC BY 4.0. · [Hugging Face](https://huggingface.co/datasets/Agentic-Payment/agent-spending-controls-crosswalk)
- [agent-spending-policy](https://github.com/Pink-Agentic-Payments/agent-spending-policy): a draft v0.1 vendor-neutral JSON Schema for an AI agent's spending policy (caps, allowlists, approval thresholds), mapped field-by-field to the crosswalk. Not a standard. CC BY 4.0 docs / Apache-2.0 code.
- [agent-spending-limit-example](https://github.com/Pink-Agentic-Payments/agent-spending-limit-example): a runnable example of enforcing an agent's spending cap before a payment tool runs, MIT.
- [sandbox-examples](https://github.com/Pink-Agentic-Payments/sandbox-examples): runnable examples (curl, Node MCP SDK, Python REST, an agent loop) for the agentic sandbox, MIT.
- [awesome-agentic-payments](https://github.com/Pink-Agentic-Payments/awesome-agentic-payments): a curated, link-verified list of agentic payment protocols, MCP servers, wallets and spending controls.
- [Agentic Payments Timeline (2024–2026)](https://github.com/Pink-Agentic-Payments/awesome-agentic-payments/blob/main/TIMELINE.md): 30 dated events, each linked to its primary source (also in [简体中文](https://github.com/Pink-Agentic-Payments/awesome-agentic-payments/blob/main/TIMELINE.zh-CN.md)).

## Learn

- [What are agentic payments?](https://pinkwallet.com/agentic/learn/agentic-payments/?utm_source=github)
- [AI agent spending controls](https://pinkwallet.com/agentic/learn/ai-agent-spending-controls/?utm_source=github)
- [x402 vs AP2 vs ACP](https://pinkwallet.com/agentic/learn/x402-vs-ap2-vs-acp/?utm_source=github)
- [Agentic Payments Readiness Report 2026](https://pinkwallet.com/agentic/research/agentic-payments-readiness-report-2026/?utm_source=github)

Website: https://pinkwallet.com/agentic/
