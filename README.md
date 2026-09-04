# part1-semester-4
# RaceDay Event Management System

## Project Overview

RaceDay is a web-based event management system designed for the South African running, walking and cycling community.

The system helps event organisers manage sporting events, categories, participant registrations and results. Participants can create an account, browse upcoming events, register for events and view their results and performance history.

The project is developed as a full-stack, API-driven application using a relational database.

## Main Features

### Organisers

Organisers can:

- Register and log in.
- Create new events.
- Update event details.
- Delete events.
- Create event categories.
- View registered participants.
- Record participant results.
- Update participant results.

### Participants

Participants can:

- Create an account.
- Log in.
- Manage their profile.
- Browse upcoming events.
- Register for events.
- View their registrations.
- View their results.
- Track their performance history.

---

## Technologies Used

- **Backend:** REST API
- **Database:** Microsoft SQL Server
- **Database Management:** SQL Server Management Studio (SSMS)
- **Data Format:** JSON
- **Database Design:** UML / ERD
- **Documentation:** Markdown

---

## Database Structure

The RaceDay database contains the following main entities:

1. `USER`
2. `ORGANISER`
3. `PARTICIPANT`
4. `EVENT`
5. `CATEGORY`
6. `REGISTRATION`
7. `RESULT`

### Relationships

- One organiser can create many events.
- One event can have many categories.
- One event can have many registrations.
- One participant can register for many events.
- One participant can have many results.
- One event can have many results.
- One category can have many results.
- One user can have an organiser or participant profile.

The `REGISTRATION` entity is used to manage the many-to-many relationship between participants and events.

---
## API Endpoints

### Authentication

```text
POST /api/auth/register
POST /api/auth/login
