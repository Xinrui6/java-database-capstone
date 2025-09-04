## MySQL Database Design
### Table: doctors 
- id: LONG, Primary Key, auto Increment
- name: String, Not Null
- Specialization: String, Not null
- email: string, not null, unique
- password: String, not null
- phone: String, not null
- role: String, not null
- avaiable_slots: List of Stringd, NOT NULL
### Table: patients
- id: Long, Primary Key, auto Increment
- name: String, not null
- email: String, not null, unique
- password: string, not null
- role: String, not null
- date_of_birth: Datetime, not null
### Table: appointments
- id: INT, Primary Key, Auto Increment
- doctor_id: INT, Foreign Key → doctors(id)
- patient_id: INT, Foreign Key → patients(id)
- appointment_time: DATETIME, Not Null
- status: INT (0 = Scheduled, 1 = Completed, 2 = Cancelled)
### Table: admin
- id: Long, Primary key, auto Increment
- username: String, not null, unique
- password: String, not null 
- role: String, not null

## MongoDB Collection Design
### Collection: prescriptions
```json
{
  "_id": "ObjectId('64abc123456')",
  "patientName": "John Smith",
  "appointmentId": 51,
  "medication": "Paracetamol",
  "dosage": "500mg",
  "doctorNotes": "Take 1 tablet every 6 hours.",
  "refillCount": 2,
  "pharmacy": {
    "name": "Walgreens SF",
    "location": "Market Street"
  }
}
