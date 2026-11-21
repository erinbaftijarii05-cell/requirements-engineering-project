# 4. Prototype

## 4.1 Journey and purpose

User: A student
What they want to do: Book an appointment with a support service
What I want to find out: If students know which service to pick, what details they need to give, and if the booking is confirmed straight away

## 4.2 Prototype screens

### Screen 1 - View Services
![Screen 1](diagrams/screen1-services.png)
Student picks which support service they need. FR-1

### Screen 2 - View Free Times
![Screen 2](diagrams/screen2-times.png)
Student sees free times for that service. FR-2, FR-9

### Screen 3 - Book Appointment
![Screen 3](diagrams/screen3-book.png)
Student checks the service and time and books it. FR-3

### Screen 4 - Time no longer free
![Screen 4](diagrams/screen4-taken.png)
If someone else took the time, the student is sent back to pick another. FR-4 (candidate)

### Screen 5 - Booking done
![Screen 5](diagrams/screen5-done.png)
Tells the student the booking is saved. FR-3, FR-7. Not sure yet if staff need to approve it

the service descriptions and times on the screens are made up examples, theyre not in the brief. in a real project id check them with the stakeholders

## 4.3 Walkthrough and findings
Self-review. I went through the screens myself as a student booking an appointment. This is not checked with real stakeholders.

| What I found | What I'll do |
|--------------|--------------|
| I don't know how long an appointment is | Added to unknowns in section 1 - Q5 |
| No rule for what info a student gives when booking | Added to unknowns in section 1 - Q6 |
| Not sure if a booking is confirmed straight away or needs staff to approve it | Added to unknowns in section 1 - Q12 and A4 |
| The student only picks a service, never a staff member | Check with support staff - Q11 |
| Reminders were not shown anywhere | Added to unknowns in section 1 - CR1 |

## 4.4 What I changed
* screen 1 was wrong, it was a copy of screen 3 so it never showed the services. made a proper one with the services list
* screen 4 said assumption for FR-4 but its candidate everywhere else now so i changed it to match
* added the question numbers to the table so you can see which ones in section 1 they link to
