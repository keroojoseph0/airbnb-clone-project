# DataScape: Mastering Database Design

## Define Entities and Relationships in ER Diagram

     ┌────────────┐       1 ──────── N       ┌────────────┐
     │    User    │──────────────────────────>│  Property  │
     │------------│                           │------------│
     │ user_id(PK)│                           │ property_id│
     │ role       │                           │ host_id(FK)│
     └────────────┘                           └────────────┘
           │ 1                                          │1
           │                                            │
           │                                            │
           │ N                                          │N
     ┌────────────┐       1 ──────── 1       ┌────────────┐
     │  Booking   │──────────────────────────>│  Payment   │
     │------------│                           │------------│
     │ booking_id │                           │ payment_id │
     │ property_id│                           │ booking_id │
     │ user_id(FK)│                           │ amount     │
     └────────────┘                           └────────────┘
           │
           │
           │N
           │
           │1
     ┌────────────┐
     │   Review   │
     │------------│
     │ review_id  │
     │ property_id│
     │ user_id(FK)│
     │ rating     │
     └────────────┘

![Airbnb Schema](https://github.com/user-attachments/assets/5080fdf0-853c-4e8a-a6e8-00efdcd7aa41)
