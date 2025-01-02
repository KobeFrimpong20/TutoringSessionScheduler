# Tutoring Session Scheduler

## Virgin Software
**Contributors:** Drew Glen, Carter Cavalier, Ben Amon-Kotey, Kobe Frimpong

### Abstract

The Tutoring Session Scheduler is designed to provide users with a simple interface which allows
students and parents to **schedule their _preferred_ tutors** and allows Tutoring Centers to **view,
confirm, and log meeting schedules.** 

### Specifcation

#### Tech Stack 

```mermaid
flowchart RL
subgraph Front End
	A(Typescript: React)
end
	
subgraph Back End
	B(Python: Flask)
end
	
subgraph Database
	C[(MySQL)]
end

A <-->|"REST API"| B
B <-->|SQLAlchemy| C
```

#### ER Diagram 

```mermaid
---
title: Database ERD
---
erDiagram
    User {
        int user_id PK
        string username
        string password_hash
        string role FK
    }

    Role {
        int role_cd PK
        string name
    }

    Meeting {
        int meeting_id PK
        int start_time
        int end_time 
        string instructor
        string[] students
    }

    Schedule {
        int schedule_id PK
        Meeting[] meetings
        string owner FK
    }

    User ||--|{ Role : HAS
    User ||--|| Schedule : OWNS
    Schedule ||--|{ Meeting : Contains
```
