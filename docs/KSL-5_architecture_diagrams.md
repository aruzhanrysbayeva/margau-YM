# KSL-5: Architecture Diagrams

Project: margau-YM, a mobile application for learning Kazakh Sign Language (KSL).

Editable source: [`KSL-5_architecture_diagrams.drawio`](KSL-5_architecture_diagrams.drawio) (draw.io, 3 pages: System Context, Use Case, Component).

The diagrams below are rendered by GitHub from Mermaid code. Dashed elements are optional or potential, not part of the mandatory MVP.

---

## Figure 1. System Context Diagram

```mermaid
flowchart LR
    L(["Learner"])
    S["<b>margau-YM</b><br/>Mobile Application<br/>(system under development)"]
    B["<b>Backend Services</b><br/>(structured data)"]
    V["<b>Video Storage Service</b><br/>(educational videos)"]
    A["<b>Content Administrator</b><br/>(potential role)<br/>via backend tools in v1"]

    L -->|"browses lessons,<br/>completes quizzes"| S
    S -->|"video demonstrations,<br/>feedback, progress"| L
    S -->|"requests / saves data"| B
    S -->|"streams video files"| V
    A -.->|"manages content"| B
    A -.->|"uploads videos"| V

    style S fill:#DBEAFE,stroke:#2563EB,stroke-width:3px
    style B fill:#DCFCE7,stroke:#16A34A,stroke-width:2px
    style V fill:#FEF3C7,stroke:#D97706,stroke-width:2px
    style A fill:#F3E8FF,stroke:#7C3AED,stroke-width:2px,stroke-dasharray: 5 5
```

| Element | Type | Description |
| --- | --- | --- |
| Learner | Actor | Browses lessons, completes quizzes, receives video demonstrations, feedback and progress |
| margau-YM Mobile Application | System under development | Main system |
| Backend Services | External service | Stores structured data (categories, lessons, questions, progress) |
| Video Storage Service | External service | Stores and streams educational videos |
| Content Administrator | Potential role (dashed) | Manages content and uploads videos via backend tools in v1 |

---

## Figure 2. Use Case Diagram

```mermaid
flowchart LR
    L(["Learner"])

    subgraph SYS["margau-YM"]
        direction TB
        subgraph MVP["MVP (mandatory)"]
            direction TB
            U1(["Browse learning categories"])
            U2(["Select lesson"])
            U3(["Watch video demonstration"])
            U4(["Complete quiz"])
            U5(["Receive feedback"])
            U6(["View learning progress"])
        end
        subgraph OPT["Optional"]
            direction TB
            U7(["Search sign dictionary"])
            U8(["Review completed lessons"])
            U9(["Verify gesture using camera"])
        end
    end

    L --- U1
    L --- U2
    L --- U3
    L --- U4
    L --- U6
    U2 -.->|"«include»"| U3
    U4 -.->|"«include»"| U5
    L -.->|"optional features<br/>(not part of MVP)"| OPT

    style OPT stroke-dasharray: 5 5
```

| Use case | Scope | Related requirement |
| --- | --- | --- |
| Browse learning categories | MVP | FR-01 |
| Select lesson | MVP | FR-02 |
| Watch video demonstration | MVP | FR-03 |
| Complete quiz | MVP | FR-04 |
| Receive feedback | MVP | FR-05 |
| View learning progress | MVP | FR-06, FR-07 |
| Search sign dictionary | Optional | FR-09 |
| Review completed lessons | Optional | FR-10 |
| Verify gesture using camera | Optional | FR-12 |

Relationships: *Select lesson* includes *Watch video demonstration*; *Complete quiz* includes *Receive feedback*.

---

## Figure 3. Component Diagram

```mermaid
flowchart TB
    subgraph APP["Mobile Application"]
        direction TB
        NAV["Navigation"]
        LC["Learning Content"]
        QZ["Quizzes"]
        PT["Progress Tracking"]
        MS["Mascot Interaction"]
        DAL["Data-Access Layer"]
    end

    subgraph BE["Backend Services"]
        direction LR
        DB[("Database<br/>categories, lessons,<br/>questions, user progress")]
        ST["Storage Service<br/>(educational video files)"]
    end

    NAV --> LC
    NAV --> QZ
    NAV --> PT
    QZ -->|"feedback"| MS
    PT -->|"encouragement"| MS
    LC --> DAL
    QZ --> DAL
    PT --> DAL
    DAL -->|"queries / saves data"| DB
    DAL -->|"streams video files"| ST
```

| Component | Responsibility |
| --- | --- |
| Navigation | Moves the learner between learning content, quizzes and progress |
| Learning Content | Shows categories, lessons and video demonstrations |
| Quizzes | Runs quizzes and evaluates answers |
| Progress Tracking | Records completed lessons and quiz results, shows progress |
| Mascot Interaction | Cat mascot: gives feedback after quizzes and encouragement for progress |
| Data-Access Layer | Single access point to the database and storage service |
| Database | Categories, lessons, questions, user progress |
| Storage Service | Educational video files |

> Architecture decisions (React Native + Expo, Supabase, Supabase Storage) are preliminary, see `KSL-4_system_technology_comparison.md`.
