# Paws: Client Inbox Coordinator

A hackathon prototype exploring how a small veterinary clinic in Cairo, Egypt, could organize incoming client messages through a Telegram bot. The workflow uses Make.com to classify inquiries, respond to suitable administrative questions, and flag potentially urgent messages for human attention.

This is an early-stage prototype, not a production veterinary service. Message classification and response quality can be inconsistent, especially for ambiguous clinical inquiries, and further testing is needed.

---

## Project Overview

Small veterinary clinics receive a mixture of administrative questions and messages that may require veterinary attention. Manually monitoring these messages can add to staff workload and make it harder to prioritize inquiries, including after hours.

Paws explores a low-cost, AI-assisted workflow that helps organize incoming messages while keeping veterinary decisions under human oversight.

## Problem

The prototype focuses on three operational challenges:

- **After-hours message handling:** Clinics may receive routine questions and potentially urgent inquiries outside regular business hours.
- **Manual triage workload:** Staff need to distinguish administrative requests from messages that require veterinary attention.
- **Prioritization:** Potentially urgent messages need to be made visible to a human rather than treated as ordinary FAQs.

These are the problems the prototype is designed to explore; the project has not yet measured time saved, staff burnout reduction, or financial impact in a real clinic.

## Target Users

1. **Small veterinary clinics in Cairo:** Clinics exploring affordable ways to organize incoming client inquiries.
2. **Veterinarians and clinic staff:** People who need potentially urgent messages brought to their attention.
3. **Pet owners:** Clients contacting the clinic with administrative questions or concerns about their pets.

## Solution

Paws uses a Telegram bot as the messaging interface and Make.com to automate parts of the inquiry-handling workflow.

The current prototype can automatically respond to suitable FAQ-type messages. When a message is classified as urgent, it sends an acknowledgement to the client and alerts the designated veterinary contact with the message context.

The workflow is a prototype and requires further testing to improve classification consistency and handling of ambiguous clinical messages.

## How the Agent Works

1. **Message received:** A pet owner sends a free-form message to the Telegram bot.
2. **Classification:** The workflow processes the message and classifies it as `FAQ`, `Urgent`, or `Can-wait`.
3. **FAQ:** Suitable administrative questions can receive an automatic reply based on the clinic information configured in the workflow.
4. **Urgent:** The client receives an acknowledgement, and the designated veterinary contact receives an alert containing the message context.
5. **Can-wait or unclear messages:** Handling depends on the configured workflow behavior. These cases need additional testing to ensure they are consistently routed for human review.

## Technology

- **Telegram Bot:** Client-facing messaging and the current testing channel.
- **Make.com:** Workflow automation and routing.
- **AI service:** Used by the configured Make.com scenario for message classification. The specific provider should be confirmed in the active scenario.
- **Data logging:** Only describe or rely on logging features that are currently configured and verified in the live scenario.

WhatsApp integration is not implemented in this version.

## Safety Principles

- The agent is not intended to diagnose, prescribe medication, or recommend treatment.
- Clinical decisions should remain with a qualified veterinary professional.
- Potentially urgent messages should be brought to human attention.
- Administrative auto-replies should be limited to information approved for the clinic.
- Ambiguous clinical inquiries require careful handling and further testing; the prototype should not be treated as a substitute for veterinary assessment.

## Testing the Prototype

1. Open Telegram and find the configured demo bot: **@pawsclinic_bot**.
2. Start the bot with `/start`, if prompted.
3. Send a simple administrative question, such as: `What are your opening hours?`
4. Send a potentially urgent example, such as: `My puppy was hit by a car and is bleeding heavily.`
5. Observe the client response and, for an urgent message, check whether the configured veterinary contact receives an alert.
6. **Open the Live Sheets Log:** Access publicly visible Google Sheets Live Audit Log to watch incoming data populate in real-time.

**Make.com scenario:** View the shared scenario

## Limitations

- This is a hackathon prototype for a hypothetical clinic, not a production veterinary service.
- Classification and response quality may vary, particularly for ambiguous clinical messages.
- The human-review process and Can-wait handling require further validation.
- The prototype currently uses Telegram; WhatsApp integration is not implemented.
- No real-clinic evaluation has been conducted, so time savings, cost savings, and other business outcomes have not been measured.
- Availability of the bot and scenario depends on the relevant services, configuration, and access permissions.

## Future Improvements

- Test a broader set of English and Egyptian Arabic messages, including ambiguous cases.
- Improve the fallback behavior for uncertain or clinical messages.
- Add and verify a reliable human-review queue and message log.
- Measure classification performance and estimate operational impact using a documented test set.
- Explore a future WhatsApp integration after the Telegram prototype is more reliable.

## Demo Video

Watch the triage demo video
