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
