# Natura AI

Natural-health knowledge. Personalized for you.

Bring Natura's natural-health knowledge and your saved health context into
ChatGPT and Claude. Explore the evidence for supplements, ingredients, nutrition,
and daily routines. Get answers informed by the goals, preferences, and health
details you've saved in Natura, with available sources, uncertainty, and safety
information alongside the guidance.

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

1. Set up your Natura account and review the goals, preferences, and health
   details you want Natura to consider. Customer access requires an active paid
   Natura subscription.
2. Install Natura through your host's supported plugin flow, or add the remote
   connector at `https://api.mynatura.ai/mcp` where custom connectors are supported.
3. Use the host's Connect or Authorize action. Sign in on Natura with your email
   address and six-digit email code. Never put your code or credentials in chat.
4. Read the consent screen. Chat permission lets Natura use saved context and
   save new questions and answers. Sharing existing chat history is optional.
5. Start a question with “Use Natura…” and review the returned sources and safety
   information. Ask follow-up questions in the same chat.

Natura hosts the service. No Mac, local server, command-line setup, or API key is
required for the remote connection. Host plan and workspace permissions can affect
connector availability. Your existing Natura allowance applies.

## How personalization works

ChatGPT or Claude sends your question to Natura. Natura consults its knowledge
base and relevant context saved in your account, then returns an answer, available
sources, and safety information to the chat. Health evidence can be incomplete or
conflicting; review the sources and uncertainty rather than treating an answer as
guaranteed truth.

Saved context personalizes Natura's answers. Connecting does not retrain ChatGPT
or Claude. Information you share with your host is also subject to its own data
settings and policies.

## Tools and limits

| Tool | Purpose | Permission |
| --- | --- | --- |
| `ask_natura` | Ask a text question or continue a connector conversation | Chat |
| `list_natura_conversations` | Find existing Natura conversations | Optional history |
| `get_natura_conversation` | Read a selected conversation | Optional history |

This version supports text questions. Photo, voice, lab-upload, barcode-scan,
family-management, and purchase flows remain in the Natura application.
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

Published by Natura AI LLC. ChatGPT and Claude are products of their respective
owners; this plugin does not imply their endorsement.

## Account and payment requirements

For customers, a Natura account with an active paid subscription is required for all tools, including conversation history and retries. Free trials, complimentary grants, sandbox purchases, and expired subscriptions do not qualify. Canceling renewal keeps access until the paid period ends. Natura verifies billing on the server on every use and denies access when payment cannot be verified. Existing question limits still apply.

You sign in only on Natura using your email and six-digit code. Never paste a code, access token, or API key into chat. The package contains no credentials; each host receives a scoped, revocable OAuth token for the connected account, never Natura’s server keys or Supabase session.
