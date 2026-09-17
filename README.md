# AI Lead Qualification Telegram Bot

A no-code AI automation project built with **Make.com, OpenAI, and Telegram** to capture incoming leads, guide them through a qualification flow, store structured information, and hand qualified leads over to a manager.

The project was created as a practical business automation demo focused on lead handling, conversational logic, data collection, and human handoff.

## What the Workflow Does

- Receives incoming messages from Telegram
- Handles both button-based and free-text conversations
- Guides users through city, service, extras, and preferred date selection
- Uses OpenAI to understand free-text messages and answer questions
- Collects lead information step by step
- Stores conversation state and structured lead data
- Routes users through different paths using filters and conditional logic
- Validates user input in multi-step flows
- Shows a final lead summary before confirmation
- Supports prepayment confirmation logic
- Sends qualified lead information to a manager
- Supports human handoff after qualification

## My Role

I designed and built the automation workflow, including:

- Conversation flow and routing logic
- Make.com routers, filters, and conditional branches
- Lead data collection and qualification logic
- OpenAI integration for free-text conversations
- Telegram Bot interaction flow
- State management and structured data storage
- Input validation and fallback handling
- Manager notifications and human handoff
- Testing, debugging, and workflow improvements

## Tools & Technologies

- **Make.com** — workflow automation, routers, filters, conditions, and scenario logic
- **OpenAI** — AI-powered understanding and free-text responses
- **Telegram Bot API** — user communication and bot interaction
- **Make Data Store** — state management and structured lead data
- **Webhooks** — event-driven automation
- **Conditional logic** — routing users through different conversation paths

## Workflow Architecture

```text
Telegram User
    ↓
Telegram Bot
    ↓
Make.com
    ↓
Routing & Filters
    ↓
Data Collection + State Management
    ↓
OpenAI for Free-Text Handling
    ↓
Lead Qualification
    ↓
Confirmation / Prepayment Step
    ↓
Manager Notification + Human Handoff
```

## Example User Flow

```text
/start
  ↓
Choose city
  ↓
Choose service
  ↓
Choose extras
  ↓
Choose date / time
  ↓
Review collected information
  ↓
Confirm details
  ↓
Prepayment confirmation
  ↓
Manager handoff
```

The bot also includes a fallback AI route so that users can write their own messages instead of being limited to menu buttons.

## Key Features

- Conversational lead qualification
- Button-based and free-text interactions
- Multi-step data collection
- Structured lead information
- State-based conversation logic
- Automated routing
- Input validation
- AI fallback responses
- Manager notifications
- Human handoff
- Lead summary before final confirmation

## Project Goal

The goal was to automate the first stage of customer communication so a business can:

- respond to leads faster
- collect useful information automatically
- reduce repetitive manual communication
- keep lead data structured
- pass qualified prospects to a manager with the necessary context

## What I Learned

This project gave me practical experience with:

- designing multi-step automation workflows
- working with structured data and state management
- debugging conditional branches and filters
- integrating AI into business processes
- validating user input
- designing fallback logic for unpredictable user messages
- combining automation with human handoff

## Screenshots

Project screenshots of the Make.com workflow and Telegram bot conversation will be added here.

## Security

API keys, bot tokens, webhook secrets, private credentials, and real customer data are **not included** in this public repository.

## Status

The project is functional and has been tested across the main qualification flow, including free-text handling, structured data collection, confirmation logic, and manager handoff.
