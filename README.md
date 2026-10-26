# Natura AI

Give your AI a natural health upgrade. Connect Natura to your AI chat for
natural-health questions grounded in Natura's knowledge base, with source-aware
answers, evidence limitations, safety checks, and your saved Natura health context.

This integration is being prepared for directory review. Installing this package
does not by itself activate a Natura account or guarantee directory availability.

## What you can ask

- “Use Natura to explain the evidence for magnesium and sleep, including sources
  and important cautions.”
- “Use Natura to review an ingredient list. Ask me to paste the ingredients.”
- “Use Natura to help me build an evening routine around my saved goals.”
- With optional history access: “Find my recent Natura conversation and help me
  continue it.”

## Connect your account

1. Install Natura through your host's supported plugin flow, or add the remote
   connector at `https://api.mynatura.ai/mcp` where custom connectors are supported.
2. Use the host's Connect or Authorize action. Sign in on Natura with your email
   address and six-digit email code. Never put your code or credentials in chat.
3. Read the consent screen. Chat permission lets Natura use saved context and
   save new questions and answers. Sharing existing chat history is optional.
4. Ask a question and review the returned sources and safety information.

Natura hosts the service. No Mac, local server, command-line setup, or API key is
required for the remote connection. Host plan and workspace permissions can affect
connector availability. Your existing Natura allowance applies.

## Tools and limits

| Tool | Purpose | Permission |
| --- | --- | --- |
| `ask_natura` | Ask a text question or continue a connector conversation | Chat |
| `list_natura_conversations` | Find existing Natura conversations | Optional history |
| `get_natura_conversation` | Read a selected conversation | Optional history |

This version supports text questions. Photo, voice, lab-upload, barcode-scan,
family-management, and purchase flows remain in the Natura application.
Connecting adds access to Natura's service; it does not retrain the host model.
Natura provides general wellness information, not diagnosis or treatment, and
does not replace a qualified clinician or emergency care.

## Privacy and disconnecting

Questions and tool results pass between the host and Natura. Natura may use your
saved health context to answer; complete existing conversations are shared only
with optional history permission. New questions and answers are saved to your
Natura account. Only share information you intend both services to receive.

[Review saved context](https://app.mynatura.ai/memories) and
[disconnect a linked app](https://app.mynatura.ai/account/connections) in Natura.
Disconnecting prevents future connector access; it does not erase information
already received by your AI host. Data retention and deletion follow the
[Natura privacy policy](https://mynatura.ai/privacy), along with the host's own
policy for data it receives. Account and health data are retained while your
account is active; Natura's privacy policy describes deletion requests and
applicable legal exceptions.

The public package contains configuration, instructions, and branding, not
Natura's private backend, knowledge base, user data, or credentials.

## Support

- [Natura](https://mynatura.ai)
- [Help](https://mynatura.ai/help)
- [Terms](https://mynatura.ai/terms)
- Support: support@mynatura.ai
- Privacy: privacy@mynatura.ai

Published by Natura AI. ChatGPT and Claude are products of their respective
owners; this plugin does not imply their endorsement.
