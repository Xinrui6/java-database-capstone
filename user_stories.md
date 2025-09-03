## Admin User Stories
**Title: Admin Secure Login**
_As an Admin, I want to log into the portal with my username and password, so that I can manage the platform securely._
**Acceptance Criteria:**
1. The login page must have fields for username and password.
2. Upon successful authentication, I am redirected to the Admin Dashboard.
3. If authentication fails, a clear error message is displayed.
**Priority:** high
**Story Points:** 2
**Notes:**
- Implement security measures against brute-force attacks.

**Title: Admin Secure Logout**
As an Admin, I want to log out of the portal, so that I can protect system access when I am finished with my session._
**Acceptance Criteria:**
1. A "Logout" button is clearly visible within the authenticated portal.
2. Clicking "Logout" invalidates my session.
3. After logging out, I am redirected to the public login page.
**Priority:** high
**Story Points:** 1
**Notes:**
- Ensure no sensitive pages can be accessed using the browser's back button after logout.

**Title: Add New Doctor**
As an Admin, I want to add doctors to the portal, so that the roster of available medical professionals is up-to-date._
**Acceptance Criteria:**
1. There is an "Add Doctor" form in the admin dashboard.
2. The form includes fields for the doctor's name, specialization, email, and a temporary password.
3. Upon submission, the new doctor's profile is created and visible in the list of doctors.
**Priority:** high
**Story Points:** 3
**Notes:**

**Title: Delete Doctor Profile**
As an Admin, I want to delete a doctor's profile from the portal, so that I can remove staff who are no longer with the clinic.
**Acceptance Criteria:**
1. There is an option to delete a doctor from the list of doctors.
2. A confirmation modal appears before the deletion is finalized to prevent accidental removal.
3. Once confirmed, the doctor's profile is removed from the system.
**Priority:** Medium
**Story Points:** 2
**Notes:**

**Title: View Monthly Appointment Statistics**
As an Admin, I want to view the number of appointments per month, so that I can track usage statistics and platform growth.
**Acceptance Criteria:**
1. There is a "Reports" or "Dashboard" section accessible to admins.
2. This section displays a chart or table showing the total number of appointments for each of the last 6-12 months.
3. The data accurately reflects the appointment records in the database.
**Priority:** Medium
**Story Points:** 5
**Notes:**

## Patient User Stories
**Title: View Doctor List (Unauthenticated)**
As a prospective patient, I want to view a list of doctors without logging in, so that I can explore my options before registering for an account.
**Acceptance Criteria:**
1. The public homepage or a "Doctors" page shows a list of all active doctors.
2. Each doctor's listing includes their name and specialization.
3. I do not need to be logged in to see this information.
**Priority:** High
**Story Points:** 2
**Notes:**

**Title: Patient Account Signup**
As a new user, I want to sign up using my email and password, so that I can create an account to book appointments.
**Acceptance Criteria:**
1. A "Sign Up" page with fields for name, email, and password is available.
2. The system validates that the email is unique.
3. Upon successful registration, I am logged in and redirected to my dashboard.
**Priority:** High
**Story Points:** 3
**Notes:**

**Title: Patient Secure Login/Logout**
As a Patient, I want to log in and out of the portal, so that I can securely manage my bookings and protect my account.
**Acceptance Criteria:**
1. I can log in using the email and password I registered with.
2. A "Logout" button is available after I log in.
3. Logging out ends my session and returns me to the login page.
**Priority:** High
**Story Points:** 2
**Notes:**

**Title: Book an Appointment**
As a Patient, I want to book an hour-long appointment with a doctor, so that I can schedule a consultation.
**Acceptance Criteria:**
1. After logging in, I can select a doctor and view their available time slots.
2. The system only shows time slots that the doctor has marked as available.
3. I can select a date and time slot, confirm my choice, and the appointment is created.
**Priority:** High
**Story Points:** 8
**Notes:**

**Title: View Upcoming Appointments**
As a Patient, I want to view my upcoming appointments, so that I can prepare for them accordingly.
**Acceptance Criteria:**
1. My user dashboard displays a section for "Upcoming Appointments."
2. This section lists the doctor's name, date, and time for each future appointment.
3. If I have no upcoming appointments, a message indicates this.
**Priority:** High
**Story Points:** 3
**Notes:**

## Doctor User Stories
**Title: Doctor Secure Login/Logout**
As a Doctor, I want to log in and out of the portal, so that I can securely manage my schedule and protect patient data.
**Acceptance Criteria:**
1. I can log in with the credentials provided by the admin.
2. A "Logout" button is always accessible within the portal.
3. Logging out securely ends my session.
**Priority:** High
**Story Points:** 2
**Notes:**

**Title: View Appointment Calendar**
As a Doctor, I want to view my appointment calendar, so that I can stay organized and know my schedule.
**Acceptance Criteria:**
1. My dashboard displays a calendar or list view of my scheduled appointments.
2. I can easily view appointments for today, this week, and this month.
3. Each entry shows the patient's name and the appointment time.
**Priority:** High
**Story Points:** 3
**Notes:**


**Title: Manage Availability**
As a Doctor, I want to mark my unavailability, so that patients can only book appointments in my available slots.
**Acceptance Criteria:**
1. I have a schedule management interface (e.g., a weekly calendar).
2. I can block off specific days or time ranges (e.g., for vacation or lunch).
3. Any time I mark as unavailable is immediately removed from the patient booking view.
**Priority:** High
**Story Points:** 5
**Notes:**


**Title: Update Doctor Profile**
As a Doctor, I want to update my profile with my specialization and contact information, so that patients have the most up-to-date information about me.
**Acceptance Criteria:**
1. There is an "Edit Profile" section in my dashboard.
2. I can change fields like my specialization, phone number, and a short bio.
3. Saving the changes updates my public-facing profile that patients see.
**Priority:** Medium
**Story Points:** 2
**Notes:**

**Title: View Patient Details for Appointment**
As a Doctor, I want to view the patient details for my upcoming appointments, so that I can be prepared for each consultation.
**Acceptance Criteria:**
1. I can click on an appointment in my calendar to see more details.
2. The detail view shows the patient's name and any reason for the visit they provided.
3. A link to the patient's full medical history (within our clinic) is also available.
**Priority:** High
**Story Points:** 3
**Notes:**

