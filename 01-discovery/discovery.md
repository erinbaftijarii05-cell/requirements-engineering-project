# Week 1 — Initial Discovery
Scenario: College Equipment Booking System (worked example)

## 1. Facts
- Students and staff share equipment such as laptops, cameras, projectors and specialist equipment.
- Bookings are currently managed using email, spreadsheets and informal arrangements.
- Equipment can be double-booked.
- People are sometimes unsure whether equipment is available.
- Staff spend time checking bookings manually.
- Equipment is not always returned when expected.
- Students are not always sure who to contact about equipment.

## 2. Assumptions
- All students and staff have a college login.
- Each item is lent to one person at a time.
- Bookings are made in advance, not only on the day.
- One team manages all the equipment.

## 3. Unknowns
- Who is allowed to book specialist equipment?
- How far in advance can equipment be booked?
- What happens when equipment is returned late or damaged?
- Do bookings need to be approved by someone?

## 4. Stakeholders
| Stakeholder | What might they need or care about? | Why included |
|---|---|---|
| Student | Seeing availability, booking easily | Main borrower (scenario) |
| Lecturer | Equipment ready for classes | "Staff" also book (scenario) |
| Equipment technician | Knowing what is out and due back | Deals with returns |
| Equipment manager | Accountability, avoiding losses | Responsible for the stock |
| Department administrator | Accurate records | Keeps the spreadsheets today |

**Conflict:** lecturers may want priority for teaching, while students expect first come, first served.

## 5. Goals
- The system should help the college to prevent the same item being double-booked.
- The system should help the college to show availability before someone books.
- The system should help the college to track when equipment is due back.

## 6. Scope
**In scope (likely):**
- viewing equipment availability
- making a booking
- recording when equipment is returned
- seeing what is due back

**Out of scope / not established:**
- buying new equipment
- repairs
- fines for late returns

## 7. Candidate Requirements
*Candidate requirements — still need investigation and validation.*

| ID | Requirement |
|---|---|
| FR1 | The system shall allow an authorised user to view equipment availability for a selected date. |
| FR2 | The system shall prevent an item being booked for overlapping periods. |
| FR3 | The system shall record the expected return date for each booking. |
| FR4 | The system shall allow a technician to record when an item is returned. |
| NFR1 | Only users signed in with a college account shall be able to make a booking. |
| NFR2 | Availability for a selected date shall be shown within 3 seconds. |

## 8. Requirement Surgery
**R1: "The system should be easy to use."**
- Why weak: "easy" is subjective. It doesn't say easy for whom, for which task, or how to measure it.
- Rewrite: A first-time student shall be able to book an available item in under 3 minutes without help.

**R2: "The system should be secure."**
- Why weak: it doesn't say what we are protecting, from whom, or how to check it.
- Rewrite: Only signed-in college users shall be able to make bookings, and only equipment technicians shall be able to mark an item as returned.

## 9. Reflection
- I wanted to jump straight to a solutionbut listing the unknowns first showed how much we don't know yet, and would like who can book specialist equipment and what happens with late returns
-words like "easy" and "secure" sound fine but can't be tested until you ask wh
