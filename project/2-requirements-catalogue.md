# 2. Requirements 

* These are my first requirements and They still need to be checked with the stakeholders

  ## 1. Functional Requirements
| ID    | Requirement                                                                                          | Type       |Priority|Source           | why                     | Verification    |
|-------|------------------------------------------------------------------------------------------------------|------------|-------|------------------|---------------------------------|----------------------------|
| FR-1  | The system shall allow students to view all support services available in the college                | Functional | Must  | Scenario         | Don't know where to go          | List shows                 |
| FR-2  | The system shall allow students to view the available appointment times for a chosen support service | Functional | Must  | Scenario         | Can't see free times            | Times show                 |
| FR-3  | The system shall allow students to book an available appointment time with a chosen support service  | Functional | Must  | Scenario         | No more emails                  | Booking saves              |
| FR-4  | The system shall prevent two students from booking the same appointment time                         | Functional | Must  | Candidate - to confirm | Clashes                         | Taken time fails           |
| FR-5  | The system shall allow students to cancel their own bookings                                         | Functional | Must  | Scenario         | Hard to cancel now              | Booking removed            |
| FR-6  | The system shall allow students to change the time of their own bookings                             | Functional | Should| Scenario         | Hard to change now              | Time updates               |
| FR-7  | The system shall allow students to view a list of their upcoming bookings                            | Functional | Must  | Candidate - to confirm | Know when to go                 | Bookings show              |
| FR-8  | The system shall allow support staff to view the bookings made for their support service             | Functional | Must  | Candidate - to confirm | Know who is coming              | List shows                 |
| FR-9  | The system shall allow support staff to add available appointment times for their support service    | Functional | Must  | Candidate - to confirm | Staff have different free times | New time shows to students |
| FR-10 | The system shall allow support staff to mark a booking as missed when the student does not attend    | Functional |Should |Candidate - to confirm | Scenario asks about no-shows    | Booking shows as missed    |



## 2. Business Requirements
| ID    | Requirement                                                                                                    | Type     |Priority | Source          | Why                    | How to test    |
|-------|----------------------------------------------------------------------------------------------------------------|----------|---------|-----------------|------------------------|----------------|
| BR-01 | The system shall store no personal data about students other than their name, student number and email address | Business | Must    | Candidate - to confirm |only keep what is needed| Check database |


## 3. Quality Requirements
| ID     | Requirement                                                                                               | Type          |Priority| Source                 | Why             | How to test           |
|--------|-----------------------------------------------------------------------------------------------------------|---------------|--------|------------------------|-----------------|-----------------------|
| NFR-1  | The system shall require all users to log in before they can view or make bookings                        | Security      | Must   | Scenario               | Keep others out | Try without login     |
| NFR-2  | The system shall prevent students from viewing other students' bookings                                   | Privacy       | Must   | Scenario               | Keep it private | Try another student's booking |
| NFR-3  | The system shall prevent support staff from viewing bookings for any support service other than their own | Privacy       | Must   | Candidate - to confirm | Keep it private | Try another service   |
| NFR-4  | The system shall store passwords in hashed form, never as plain text                                      | Security      | Must   | Candidate - to confirm | Stop leaks      | Check database        |
| NFR-5  | The system shall give every input field a visible label                                                   | Accessibility | Should | Scenario               | Easy for all    | Check each box        |
| NFR-6  | The system shall allow a student to complete a booking, from login to confirmation, in under 3 minutes    | Usability     | Should | Candidate - to confirm | Easy to use     | 4 of 5 students do it in under 3 mins |

## 4. Review
| What I wrote first    | What was wrong       | Changed to     |
|-----------------------|----------------------|----------------|
| Easy to use           | No way to check it   | NFR-6         |
| Secure                | Didn't say how       | NFR-1  NFR-4 |
| Staff manage bookings | Didn't say what      | FR-8 to FR-10 |

## 5. Still Need to Find Out
* How late can a student cancel -FR-5
* What do support staff do if a student does not  turn up -FR-10
* Is 3 minutes enough time to book -NFR-6

## 6. What I changed
* the ones i made up myself that arent in the brief are now marked candidate so i know to check them with the stakeholders
* the 3 minute thing is my own guess so thats a candidate too  and the test now says how many students need to pass
