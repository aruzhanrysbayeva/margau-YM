
# margau-YM — Project Proposal and Requirements

**Diploma Project:** Deployment of Mobile Application on Interactive E-Learning Platform for Kazakh Sign Language (KSL)

**Application Name:** margau-YM  
**Project Stage:** First Pre-Defense  
**Date:** October 24, 2026

---

## 1. Introduction and Background

Sign languages are natural languages with their own grammar and vocabulary, and they are the primary means of communication for many deaf and hard-of-hearing people. Most hearing people have little or no exposure to sign language, which creates a communication gap between deaf and hearing communities (Siong et al., 2021; Cabanillas-Carbonell et al., 2022).

The gap is especially significant inside families: most deaf children are born to hearing parents, who often cannot provide a signing environment at home, and late exposure to sign language can delay a child's language development (Siong et al., 2021).

Formal ways of learning sign language, such as courses and private teachers, require time, money, and travel to a learning centre, so they are not accessible to everyone (Mohammad et al., 2022; Siong et al., 2021).

Books and static images cannot show movement, while video tutorials are popular but give no feedback to the learner (Siong et al., 2021). Smartphones offer a way to close this gap: they are widely available, allow learning at one's own pace, and can combine video, quizzes, and game elements.

In Kazakhstan, Kazakh Sign Language (KSL, also referred to as Kazakh-Russian Sign Language, KRSL, in the research literature) is used by the deaf community. According to Mukushev et al. (2022), KRSL is closely related to Russian Sign Language and the two show substantial lexical overlap.

---

## 2. Problem Statement

People who want to learn KSL, such as family members of deaf people, teachers, classmates, and interested members of the public, currently lack an accessible, structured, and engaging way to do so on their own.

Although digital learning resources for Kazakh Sign Language already exist, there remains a need to investigate how structured video lessons, interactive practice, and learner-centered design can be integrated and evaluated in a coherent mobile learning environment for beginners.

---

## 3. Project Aim, Objectives, and Research Questions

### 3.1 Project Aim

To design, implement, and deploy a mobile application, **margau-YM**, on an interactive e-learning platform that helps people learn Kazakh Sign Language.

### 3.2 Project Objectives

1. Analyse existing research and sign language learning applications and identify the research gap.
2. Collect user requirements through an interview and a survey.
3. Specify requirements and design the architecture and user interface of the application.
4. Implement thematic video lessons, quizzes, and progress tracking, and evaluate the feasibility of a searchable dictionary and camera-based sign verification.
5. Deploy the application and evaluate its usability and learning potential with users.

### 3.3 Research Questions

- **RQ1:** What do potential learners and people close to the deaf community need from a KSL learning application?
- **RQ2:** Which features (thematic video lessons, tests, dictionary, sign checking) are most valuable to users?
- **RQ3:** How usable is the developed application, and what is its learning potential?

---

## 4. Project Scope and Limitations

The project focuses on a limited KSL vocabulary organised into thematic categories.

### 4.1 In Scope

- Thematic learning categories and structured lessons.
- Video demonstrations of KSL signs.
- Interactive quizzes and immediate feedback.
- Learning progress tracking.
- Integration of the margau-YM cat mascot.
- User-friendly mobile interface.
- Development and deployment of the mobile application.

### 4.2 Optional Features

- Searchable KSL sign dictionary.
- Revision of completed lessons.
- Learning streaks, achievements, and rewards.
- Camera-based verification of a limited set of signs.

### 4.3 Limitations

- The initial version will not cover the entire KSL vocabulary or grammar, including continuous signing, facial expressions, and spatial grammar.
- Camera-based sign checking is optional because recognition models are sensitive to signers, devices, and frame rates (Kim & Kim, 2024; Mukushev et al., 2022).
- The survey sample is limited to 19 responses, and the interview includes one participant. Therefore, the findings indicate potential user needs but cannot be generalized to the entire population.

---

## 5. Requirements Analysis

The requirements for margau-YM were identified through the literature review, analysis of existing applications, a semi-structured interview, and a user survey involving 19 respondents.

The findings highlighted the importance of accessible video-based instruction, structured learning content, interactive exercises, and regular practice.

In the survey:

- **16 out of 19 respondents** selected short video lessons as a preferred learning format.
- **12 respondents** selected tests and exercises.
- **13 respondents** expressed interest in camera-based gesture verification.

The interview provided further insights into the learning process, emphasizing the importance of beginning with fingerspelling and basic vocabulary, using video demonstrations instead of static images, and providing opportunities for repeated practice.

### 5.1 Requirements Prioritization

Requirements were prioritized using the **MoSCoW method**.

| Priority | Description |
|---|---|
| **Must Have** | Essential features required for the Minimum Viable Product (MVP). |
| **Should Have** | Important features that improve the learning experience but are not critical to the initial implementation. |
| **Could Have** | Additional features that may be implemented if time and resources allow. |
| **Won't Have** | Features excluded from the initial version. |

---

## 6. Functional Requirements

Functional requirements define the main operations that the margau-YM application must support.

| ID | Functional Requirement | Priority |
|---|---|---|
| FR-01 | The system shall display learning topics organized into thematic categories. | Must Have |
| FR-02 | The system shall allow users to select a topic and access its lessons. | Must Have |
| FR-03 | The system shall provide video demonstrations of selected KSL signs. | Must Have |
| FR-04 | The system shall allow users to complete interactive quizzes based on learned signs. | Must Have |
| FR-05 | The system shall evaluate quiz answers and provide immediate feedback. | Must Have |
| FR-06 | The system shall record completed lessons and quiz results. | Must Have |
| FR-07 | The system shall display the user's learning progress. | Must Have |
| FR-08 | The system shall integrate the margau-YM cat mascot into the learning interface. | Must Have |
| FR-09 | The system should provide a searchable dictionary of KSL signs. | Should Have |
| FR-10 | The system should support revision of previously completed lessons. | Should Have |
| FR-11 | The system could provide learning streaks, achievements, and motivational rewards. | Could Have |
| FR-12 | The system could verify selected gestures using the device camera. | Could Have |

The requirements focus on providing a complete beginner learning experience rather than implementing advanced recognition or translation technologies in the initial version.

---

## 7. Non-Functional Requirements

Non-functional requirements describe the quality attributes and constraints of the proposed system.

| ID | Requirement | Proposed Acceptance Criterion |
|---|---|---|
| NFR-01 | Usability | At least 80% of test participants should complete the main learning scenario without assistance. |
| NFR-02 | Performance | Topic navigation and quiz feedback should respond within 2 seconds under defined test conditions. |
| NFR-03 | Reliability | Completed lessons and quiz results should remain available after restarting the application. |
| NFR-04 | Accessibility | Instructional videos should provide readable text descriptions and subtitles where applicable. |
| NFR-05 | Compatibility | The application should operate on the selected Android and iOS test devices. |
| NFR-06 | Maintainability | Learning, quiz, progress, and content-access functionality should be organized into separate components. |
| NFR-07 | Security | User data should be protected through appropriate authentication, authorization, and secure communication. |
| NFR-08 | Content Quality | Educational sign demonstrations should be reviewed by a person with relevant KSL knowledge before publication. |

**Note:** The proposed numerical acceptance thresholds will be reviewed and finalized before implementation and testing.

---

## 8. Functional Acceptance Criteria

Acceptance criteria define the conditions under which a requirement can be considered successfully implemented.

| Requirement | Acceptance Criteria |
|---|---|
| FR-01 / FR-02 | Users can view available categories, select a topic, and access its lessons. |
| FR-03 | Selecting a lesson opens the corresponding video, which can be played and replayed. |
| FR-04 | Users can complete a quiz containing questions related to the selected topic. |
| FR-05 | The application indicates whether an answer is correct and displays appropriate feedback. |
| FR-06 | Lesson completion and quiz results are stored successfully. |
| FR-07 | The progress screen accurately displays completed lessons and learning results. |
| FR-08 | The cat mascot appears in designated learning scenarios and provides contextual feedback. |
| FR-09 | Users can search for a sign and open its corresponding learning material, if the dictionary is implemented. |
| FR-12 | If implemented, the camera verification feature can process selected supported signs and provide feedback under defined testing conditions. |

These criteria will serve as the foundation for functional testing during the implementation stage.

---

## 9. Expected Outcomes

The project is expected to deliver:

1. A functional mobile e-learning application for beginner-level Kazakh Sign Language.
2. Structured thematic learning content supported by video demonstrations.
3. Interactive quizzes with immediate feedback.
4. A system for tracking lesson completion and learning progress.
5. An integrated cat mascot supporting the learning experience.
6. A deployed application on the selected target platforms.
7. Functional and usability evaluation results.

---

## 10. Current Project Status

**Stage:** First Pre-Defense — October 24, 2026

At this stage, the project has established its research foundation, initial requirements, and preliminary design.

The functional and non-functional requirements will guide the next development stage. Implementation and evaluation results will be documented as the application is developed.

Camera-based gesture verification remains an optional feature subject to technical feasibility and available development resources.
