# Agent Middleware

Agent Middleware (AMW) is a Preview product. I am the solo maintainer, and it is pre revenue.

AMW sits in front of tools an agent calls. A scoped permit authorizes a call. A retry with the same key returns the original receipt ID. The gateway source is public under a Fair Source license (FSL-1.1-ALv2). It is source available. The spec, verifier, SDKs, integrations and examples are Apache 2.0.

This is not a promise that a remote tool runs only once or that a charge happens only once. A remote tool call that fails before dispatch is refunded and its reserved budget is released. If a crash happens after the remote effect, the reconciler later records a delivery_uncertain receipt ID for that call. A crash on a local in process tool can leave a charged record for manual review with no receipt ID.

Start here: [agent-middleware](https://github.com/agentmiddleware/agent-middleware)

Try it: [amw-demo](https://github.com/agentmiddleware/amw-demo)

Docs and site: [agentmiddleware.dev](https://agentmiddleware.dev)

Found a security issue? Please report it privately through GitHub security advisories on the affected repo.

## Examples

* [amw-demo](https://github.com/agentmiddleware/amw-demo)
* [amw-paypal-agent-demo](https://github.com/agentmiddleware/amw-paypal-agent-demo)
