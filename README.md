# LeadFlow AI — AI Lead Qualification Automation

**Portfolio project by Ihor Skyba**

AI-powered lead handling workflow built with **Make.com, OpenAI, Telegram Bot API, Data Store, routers, filters, webhooks, and human handoff logic**.

[Website](https://leadflowai1377.netlify.app) · [Instagram](https://www.instagram.com/leadflow.ai_1377/) · [GitHub Profile](https://github.com/leadflowai1377)

---

## What this project solves

Service businesses often lose leads because replies are slow, qualification is manual, and important information is scattered across chats.

This workflow automates the first stage of lead handling:

**New inquiry → qualification → structured data collection → confirmation → manager notification → human handoff**

The goal is simple: help a business respond faster, collect the right information, and pass a qualified lead to a human with context already prepared.

## What the automation does

- Receives incoming Telegram messages
- Guides a lead through city, service, extras, and preferred day selection
- Accepts free-text input where needed
- Stores conversation state and lead data in Make Data Store
- Uses routers, filters, and conditional logic to control the flow
- Validates multi-step user input
- Shows a final summary before confirmation
- Handles prepayment confirmation
- Sends structured lead information to a manager
- Supports human handoff after qualification
- Includes an experimental OpenAI fallback for free-text messages

## Workflow architecture

```text
Lead
  ↓
Telegram Bot
  ↓
Make.com
  ↓
Routers + Filters
  ↓
State Management / Data Store
  ↓
Lead Qualification
  ↓
Review + Confirmation
  ↓
Prepayment Step
  ↓
Manager Notification
  ↓
Human Handoff
```

Optional path:

```text
Free-text message → OpenAI → Telegram response
```

## Tech stack

- **Make.com** — automation orchestration
- **OpenAI** — natural-language fallback testing
- **Telegram Bot API** — lead communication
- **Make Data Store** — state and lead data
- **Webhooks / event-driven logic**
- **Routers, filters, conditions, validation**
- **Human handoff logic**

## My role

I designed, built, tested, and debugged the full workflow, including:

- Conversation flow architecture
- State-based lead qualification
- Routers and conditional branches
- Data mapping and storage
- Telegram interaction logic
- Input validation
- OpenAI integration testing
- Manager notifications
- Human handoff
- Debugging filters, routing issues, and edge cases

## Example lead flow

```text
/start
  ↓
Choose / enter city
  ↓
Choose service
  ↓
Choose extras
  ↓
Choose preferred day
  ↓
Review lead information
  ↓
Confirm
  ↓
Prepayment confirmation
  ↓
Manager handoff
```

## Project screenshots

### Complete qualification flow + manager handoff

![Complete Telegram qualification flow and manager handoff](./Снимок%20экрана%202026-09-18%20в%2010.57.21.png)

### Structured lead summary + confirmation

![Structured lead data review and confirmation](./Снимок%20экрана%202026-09-18%20в%2010.55.41.png)

### Editable qualification steps

![Telegram bot qualification navigation](./Снимок%20экрана%202026-09-18%20в%2010.56.17.png)

### Make.com AI + routing logic

![AI and routing logic](./Снимок%20экрана%202026-09-17%20в%2019.02.13.png)

### Full Make.com scenario

![Full Make.com workflow overview](./Снимок%20экрана%202026-09-17%20в%2019.01.42.png)

## Design decision: deterministic logic first

The critical qualification steps use explicit states, filters, and validation rather than relying on an LLM for every decision.

OpenAI is used only where natural-language handling can add value. Required business steps stay deterministic so the workflow remains predictable and easier to debug.

## Business use cases

The same architecture can be adapted for:

- Med Spas
- Dental clinics
- Aesthetic clinics
- Home-service businesses
- Agencies
- Appointment-based businesses
- Other service businesses receiving leads from social media or websites

Possible production channels include **Instagram, WhatsApp, websites, SMS, CRM systems, and other APIs**.

## Security

This public repository contains **no API keys, bot tokens, webhook secrets, private credentials, or real customer data**.

## Status

The core workflow is functional and tested for structured lead collection, routing, confirmation, prepayment logic, manager notification, and human handoff.

---

### LeadFlow AI

I build practical AI automation for service businesses: lead response, qualification, follow-up, CRM workflows, webhooks, APIs, and Make.com integrations.

[Visit website](https://leadflowai1377.netlify.app) · [Instagram](https://www.instagram.com/leadflow.ai_1377/)
