
# margau-YM 🐾

### Interactive Mobile Learning Application for Kazakh Sign Language

**Diploma Project:** Deployment of Mobile Application on Interactive E-Learning Platform for Kazakh Sign Language (KSL)

**University:** Astana IT University  
**Programme:** Software Engineering  
**Project Stage:** First Pre-Defense — October 24, 2026  
**Status:** Research, Requirements Analysis & System Design

---

## About the Project

**margau-YM** is a mobile e-learning application designed to support beginners in learning Kazakh Sign Language (KSL) through structured lessons, instructional videos, interactive quizzes, and gamified learning experiences.

The application aims to make introductory sign language education more accessible, engaging, and convenient for independent learners.

Inspired by interactive language-learning applications, margau-YM introduces a cat mascot that accompanies users throughout their learning journey, provides feedback, and supports learner engagement.

The project focuses on integrating educational content, practice activities, and progress tracking into a coherent mobile learning environment.

## Problem Statement

Although digital resources for Kazakh Sign Language already exist, there remains a need to investigate how structured video lessons, interactive exercises, and learner-centered design can be integrated into an effective mobile learning experience for beginners.

Traditional learning methods may require access to instructors, specialized courses, or learning materials that are not equally accessible to all potential learners.

margau-YM addresses this challenge by developing a structured, interactive mobile application for introductory KSL education.

## Target Users

The application is intended for:

- Beginners interested in learning Kazakh Sign Language.
- Family members and friends of Deaf and hard-of-hearing individuals.
- Students and teachers interested in inclusive communication.
- Individuals seeking accessible introductory KSL learning materials.

## Project Aim

To design, implement, and deploy a mobile application on an interactive e-learning platform that supports beginner-level Kazakh Sign Language learning.

## Project Objectives

1. Analyze existing research and sign language learning applications.
2. Identify user requirements through interviews and surveys.
3. Design the system architecture and user interface.
4. Develop thematic video lessons, interactive quizzes, and progress tracking.
5. Deploy the application and evaluate its usability and learning potential.

## Planned Features

### Core MVP Features

- **Thematic Learning Paths:** Lessons organized into categories such as greetings, family, numbers, and everyday communication.
- **Video Lessons:** Demonstrations of KSL signs with supporting explanations.
- **Interactive Quizzes:** Video-based questions and multiple-choice exercises.
- **Immediate Feedback:** Feedback on quiz answers and learning activities.
- **Progress Tracking:** Tracking of completed lessons and quiz results.
- **Cat Mascot:** A recognizable character providing contextual and motivational feedback.

### Additional Features

The following features may be implemented depending on technical feasibility and development resources:

- Searchable KSL sign dictionary.
- Revision of previously completed lessons.
- Learning streaks, points, and achievements.
- Camera-based gesture verification for a limited set of signs.

Camera-based verification is not part of the mandatory initial MVP.

## Proposed Technology Stack

| Component | Technology | Purpose |
|---|---|---|
| Mobile Application | React Native + Expo | Cross-platform Android and iOS development |
| Programming Language | JavaScript / TypeScript | Mobile application logic |
| Backend Platform | Supabase | Managed backend services |
| Database | PostgreSQL | Learning content, quizzes, and progress data |
| Authentication | Supabase Auth | User account management |
| Video Storage | Supabase Storage | Educational video files |
| UI/UX Design | Figma | Interface prototyping |
| Version Control | GitHub | Source control and collaboration |
| Project Management | YouTrack | Task tracking and milestones |

**Note:** The technology stack is proposed and may be refined during implementation.

## System Architecture

The proposed architecture follows a modular approach.

The mobile application will contain separate components for:

- Navigation and user interface.
- Learning content management.
- Video lesson presentation.
- Quiz processing and feedback.
- Progress tracking.
- Mascot interaction.
- Data access and backend communication.

The backend services will manage structured learning data, authentication, and educational video storage.

The system design is documented using three diagrams:

1. System Context Diagram.
2. Use Case Diagram.
3. Component Diagram.

Editable diagram source files will be maintained in the repository.

## UI/UX Prototype

A preliminary interface prototype has been created in Figma.

The prototype includes four key screens:

1. Welcome Screen.
2. Video Lesson Screen.
3. Interactive Quiz Screen.
4. Lesson Results Screen.

The design uses a consistent visual identity, a cat mascot, progress indicators, and video-based learning interactions.

**[View Figma Prototype](https://www.figma.com/design/ISmwMRteSrldLLosOePPiw/margau-YM?node-id=0-1&p=f)**

## User Research

The initial requirements were informed by:

- A semi-structured interview involving 13 questions.
- A bilingual Kazakh/Russian survey with 19 respondents.
- A literature review of 12 scientific publications.
- A comparison of Duolingo, AI-Ym, and Lingvano.

The survey indicated strong interest in short video lessons, interactive exercises, and camera-based gesture verification.

These findings were used to inform the initial functional requirements and design decisions.

## Team and Responsibilities

| Team Member | Responsibilities | YouTrack Tasks |
|---|---|---|
| Aruzhan Rysbayeva | Project proposal, requirements, user research, literature review | KSL-1, KSL-2, KSL-3 |
| Nurila Berdaly | Existing system and technology comparisons, architecture diagrams, Figma prototype | KSL-4, KSL-5, KSL-6 |

**Academic Supervisor:** Aigerim Bakiyeva

Both team members participate in planning, review activities, and preparation for project milestones.

## Project Structure

The structure will evolve as development progresses. The backend directory will be used only if custom server-side code becomes necessary.

## Documentation

Project documentation includes:

- Project proposal and scope.
- Literature review and research gap.
- Existing system comparison.
- Technology comparison and selection.
- Functional and non-functional requirements.
- Architecture diagrams.
- Figma prototype.
- Verification and evaluation plan.
- Project management and risk assessment.

See the [`docs/`](docs/) directory for available documentation.

## Project Management

Project tasks and milestones are managed through YouTrack.

**[View YouTrack Project](https://ksl-diploma.youtrack.cloud/projects/KSL)**

The repository follows a task-based Git workflow:

1. Create a YouTrack issue with an assigned owner and acceptance criteria.
2. Create a feature branch containing the issue ID.
3. Commit meaningful changes with descriptive messages.
4. Submit a Pull Request referencing the issue.
5. Request review from the other team member.
6. Merge approved changes into `main`.
7. Update the YouTrack task with the Pull Request link.

Example:

- **Task:** KSL-3 — Complete Literature Review
- **Branch:** `KSL-3-literature-review`
- **Commit:** `KSL-3: Add literature review matrix`

## Verification and Evaluation

The planned evaluation includes:

- Functional testing against requirements and acceptance criteria.
- Usability testing with beginner users.
- Measurement of task completion and navigation difficulties.
- Pre-test and post-test assessments of selected KSL vocabulary.
- Comparison with equivalent non-interactive learning materials.
- Technical testing of video playback, data persistence, and compatibility.

The proposed usability target is for at least 80% of test participants to complete the main learning scenario without assistance.

## Current Development Status

**First Pre-Defense — October 24, 2026**

The project has completed or prepared the following initial deliverables:

- Project proposal and preliminary scope.
- Literature review and research gap analysis.
- Existing system and technology comparisons.
- Initial requirements and acceptance criteria.
- Draft system architecture diagrams.
- Preliminary Figma interface prototype.
- Initial user research and findings.
- Verification and evaluation plan.
- GitHub repository and YouTrack task organization.

The application itself has not yet been implemented. The current stage focuses on research, design, technical planning, and requirements validation.

## Setup, Execution, and Testing

The application is currently in the design and planning stage.

Installation, environment configuration, execution, and automated testing instructions will be added once the first runnable version is available.

No production deployment is available at this stage.


---

**margau-YM — Making Kazakh Sign Language learning more accessible through interactive mobile education.**
```

