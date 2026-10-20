# Agent Middleware

Agents retry. Consequential tools should not run or charge twice.

Agent Middleware sits in front of the tools an agent should never call twice: refunds, payouts, writes to systems of record. Every call runs under a scoped permit, a retry with the same key returns the original receipt, and every receipt is signed with Ed25519 so anyone can verify it offline.

Start here: [agent-middleware](https://github.com/agentmiddleware/agent-middleware)
Try it: [amw-demo](https://github.com/agentmiddleware/amw-demo)
Docs and site: [agentmiddleware.dev](https://agentmiddleware.dev)

Found a security issue? Please report it privately through GitHub security advisories on the affected repo.

Agent Middleware is open source. Organization: [github.com/agentmiddleware](https://github.com/agentmiddleware)

## Examples

- [amw-demo](https://github.com/agentmiddleware/amw-demo)
- [amw-paypal-agent-demo](https://github.com/agentmiddleware/amw-paypal-agent-demo)
