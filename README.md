# Home Credit LAP Voice Agent

An AI-powered voice agent built using Retell AI to conduct preliminary qualification for Home Credit's Loan Against Property (LAP) offering.

## Project Overview

The agent conducts a structured conversation with an existing customer, collects eligibility information, checks the defined qualification criteria, and determines the appropriate next step.

This is a **preliminary qualification assistant**, not a loan approval system.

## Key Features

- Conversational qualification using Retell AI
- Property type and ownership validation
- Verification of original property document availability
- Loan amount handling with a maximum limit of ₹75 lakh
- Occupation and income-mode validation
- Property market value collection
- Loan tenure validation from 3 to 15 years
- Handling of busy customers and callback preferences
- Routing for existing loan-transfer or EMI-reduction requests
- Safe handling of failed mock identity verification
- Structured handoff to a senior loan expert

## Technology Stack

- **Voice AI Platform:** Retell AI
- **LLM:** GPT model configured in Retell AI
- **Documentation:** Notion
- **Conversation Flow:** Draw.io

## Project Documentation

- `docs/system-prompt.md` — Agent instructions and conversation rules
- `docs/conversation-flow.md` — Conversation flow and decision logic
- `docs/test-cases.md` — Test scenarios and results

## Eligibility Checks

The agent evaluates seven preliminary criteria:

1. Property type
2. Ownership type
3. Availability of original property documents
4. Requested loan amount
5. Occupation and income mode
6. Estimated current market value
7. Requested loan tenure

The agent follows the assignment's stated rules and does not invent an eligibility threshold for property market value or promise final loan approval.

## Testing

The agent has been tested against scenarios including:

- Successful preliminary qualification
- Ineligible property type
- Missing original documents
- Loan amounts above the maximum limit
- Cash-based income
- Invalid loan tenure
- Existing loan-transfer requests
- Busy-customer callback preferences
- Failed mock identity verification
- Answers provided out of order
- Joint property ownership

Test evidence should use fictional test data and must not expose real customer information or credentials.

## Important Notes

- Qualification does not guarantee loan approval.
- The senior loan expert confirms applicable interest rates and subsequent steps.
- Mock identity-verification phrases are for testing only and must not be used as real customer verification.
- No API keys, passwords, access tokens, or confidential customer recordings should be committed to this repository.

## Project Status

The Retell AI agent and initial test scenarios have been configured. Supporting documentation and submission evidence are being organized.
