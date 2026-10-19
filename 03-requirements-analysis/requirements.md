# Week 3 — Requirements Analysis and Specification
Scenario: College Equipment Booking System (worked example)

## 1. Information from Week 2
- Technicians need to know what equipment is due back.
- Lecturers need reliable availability before promising equipment to a class.
- Still unknown: who can book specialist equipment, and what happens with late returns.

## 2. Candidate Requirements — is it actually a requirement?
| Statement | Classification |
|---|---|
| A — People are sometimes unsure whether a camera is available | Problem / observation |
| B — Technicians need to know what equipment is due back | Stakeholder need |
| C — The system shall record the expected return date for each booking | Candidate requirement |
| D — The college should build a mobile app | Solution idea |
| E — We assume all users will have a college login | Assumption |
| F — A lecturer wants reliable availability information | Stakeholder need / concern |

## 3. Requirements Surgery
**Worked example: "The system shall manage bookings efficiently."**
- FIND: it's about the booking process being slow or messy.
- DIAGNOSE: "efficiently" is not measurable, and it doesn't say who or which part.
- ASK: "What part of the booking process currently causes difficulty?"
- REPAIR: The system shall allow an authorised user to view equipment availability for a selected date.
- CHECK: Select a date and confirm the list matches existing bookings.

**Requirement 1: "The system shall be user-friendly."**
- Problem: subjective. It can't be tested.
- Clarification question: Which users find the current process hardest, and at what step?
- Missing information: which users, which task, how success is measured.

**Requirement 2: "The system shall notify users about bookings."**
- Problem: doesn't say who is notified, about what, when, or how.
- Clarification question: Which booking events do users need to be told about?
- Missing information: trigger event, recipient, channel, timing.

**Requirement 3: "The system shall allow staff to create, edit and delete bookings and send reminders."**
- Problem: four separate requirements in one, and "staff" is unclear.
- Clarification question: Which staff roles should be allowed to delete a booking?
- Missing information: which staff role, under what conditions, when reminders are sent.

**Improved:** The system shall notify the borrower the day before a booked item is due to be returned.

## 4. Functional Requirements
| ID | Requirement | Source | How could we verify it? |
|---|---|---|---|
| FR-01 | The system shall allow an authorised user to view equipment availability for a selected date. | Scenario: "unsure whether equipment is available" | Select a date; check the list matches existing bookings |
| FR-02 | The system shall prevent an item being booked for a period that overlaps an existing booking of that item. | Scenario: "double-booked" | Try to make an overlapping booking; it is refused |
| FR-03 | The system shall record the expected return date for each booking. | Technician need (Week 2) | Create a booking; the return date is stored and shown |

## 5. Quality Requirements
| ID | Quality requirement | Why does it matter? | How could it be checked? |
|---|---|---|---|
| NFR-01 | Only users signed in with a college account shall be able to create a booking. | Every loan must be traceable to a person (accountability) | Try to book while signed out; the booking is refused |

## 6. Project Application — Scenario B
See the `project/` folder: `project/2-requirements-catalogue.md`.

## 7. Reflection
1. **What makes a requirement difficult to understand?** Vague words ("user-friendly", "efficiently"), not saying who is involved, and putting several requirements into one statement.
2. **What information do you still need for your project?** The rules around cancellations and no-shows, and who manages appointment availability.
3. **Who could provide that information?** Support service staff and the service administrator.
