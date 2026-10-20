# 2. Requirements 

* These are my first requirements and They still need to be checked with the stakeholders

  ## 1. Functional Requirements
| ID    | Requirement                            | Type       |Priority| Source           | why                     | Verification    |
|-------|----------------------------------------|------------|--------|------------------|-------------------------|-----------------|
| FR-1  | The system shall show all services     | Functional | Must   | Student          | Don't know where to go  | List shows      |
| FR-2  | The system shall show free times       | Functional | Must   | Student          | Can't see free times    | Times show      |
| FR-3  | A student shall book a free time       | Functional | Must   | Student          | No more emails          | Booking saves   |
| FR-4  | The system shall stop double bookings  | Functional | Must   | Support staff    | Clashes                 | Taken time fails|
| FR-5  | A student shall cancel a booking       | Functional | Must   | Student          | Hard to cancel now      | Booking removed |
| FR-6  | A student shall change a booking.      | Functional | Should | Student          | Hard to change now      | Time updates    |
| FR-7  | A student shall see their bookings     | Functional | Must   | Student          | Know when to go         | Bookings show   |
| FR-8  | Staff shall see their bookings.        | Functional | Must   | Support staff    | Know who is coming      | List shows      |



## 2. Business Requirements
| ID    | Requirement                                                | Type     |Priority | Source          | Why                    | How to test    |
|-------|------------------------------------------------------------|----------|---------|-----------------|------------------------|----------------|
| BR-01 | The system shall only save name, student number and email. | Business | Must    | Data protection |only keep what is needed| Check database |


## 3. Quality Requirements
| ID     | Requirement                                    | Type          |Priority| Source          | Why             | How to test           |
|--------|------------------------------------------------|---------------|--------|-----------------|-----------------|-----------------------|
| NFR-1  | Users shall log in first                       | Security      | Must   | Data protection | Keep others out | Try without login     |
| NFR-2  | Students shall only see their own bookings     | Privacy       | Must   | Student         | Keep it private | Try another studenyts |
| NFR-3  | Staff shall only see their own service         | Privacy       | Must   | Data protection | Keep it private | Try another service   |
| NFR-4  | Passwords shall be hidden                      | Security      | Must   | Data protection | Stop leaks      | Check database        |
| NFR-5  | Every box shall have a label                   | Accessibility | Should | Student         | Easy for all    | Check each box        |
| NFR-6  | Booking shall take under 3 minutes             | Usability     | Should | Student         | Easy to use     | Time 5 students       |

## 4. Review
| What I wrote first    | What was wrong       | Changed to     |
|-----------------------|----------------------|----------------|
| Easy to use           | No way to check it   | NFR-06         |
| Secure                | Didn't say how       | NFR-01  NFR-04 |
| Staff manage bookings | Didn't say what      | FR-08 to FR-10 |

## 5. Still Need to Find Out
* How late can a student cancel (FR-05)
* What do staff do if a student does not  turn up(FR-10)
* Is 3 minutes enough time to book? ((NNFR-06)


