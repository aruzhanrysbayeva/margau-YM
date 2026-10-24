
# margau-YM — User Research and Findings

**Diploma Project:** Deployment of Mobile Application on Interactive E-Learning Platform for Kazakh Sign Language (KSL)

**Application Name:** margau-YM  
**Project Stage:** First Pre-Defense  
**Date:** October 24, 2026

---

## 1. Methodology

The project follows an iterative, task-based development approach tracked through YouTrack and GitHub.

Requirements were collected using two methods:

1. **Semi-structured interview:** One interview conducted in Kazakh with a participant who has personal experience communicating with Deaf family members.
2. **Online survey:** A bilingual (Kazakh and Russian) Google Forms questionnaire involving 19 respondents.

Both methods were used to identify potential user needs, learning preferences, and requirements for the proposed application.

The collected data represents a convenience sample and cannot be generalized to the entire Deaf community or the wider population.

Planned verification activities include:

- Requirement-based functional testing.
- A small moderated usability study.
- Pre-test and post-test learning assessments.
- Comparison against equivalent static learning materials.

Detailed evaluation procedures and acceptance thresholds will be finalized before implementation testing.

---

## 2. Interview Results

### 2.1 Interview Overview

A semi-structured interview was conducted in Kazakh to understand the experience of learning and using sign language.

The interview consisted of **13 questions** covering:

- Previous experience with sign language.
- Difficulties encountered during learning.
- Availability of learning resources.
- Recommended order of learning topics.
- Effective exercises and practice methods.
- Opinions on the proposed margau-YM application.

The participant grew up with a deaf brother and a hard-of-hearing sister and learned basic signs during childhood to communicate with family members.

### 2.2 Key Interview Findings

The interview highlighted the importance of video-based demonstrations, feedback, fingerspelling, and regular practice.

| Theme | Participant's Experience or Opinion | Implication for margau-YM |
|---|---|---|
| Learning Path | The participant learned letters and words from a picture book and through communication with family members. | Begin with fingerspelling and basic vocabulary. |
| Beginner Mistakes | Static pictures can be misinterpreted, and direct correction from another person makes learning easier. | Provide video demonstrations and consider feedback on signing. |
| Learning Difficulties | The participant experiences difficulties constructing sentences and communicating complex meanings. | Introduce phrases after basic signs and seek content validation. |
| Sign Language Grammar | The participant observed differences in sentence structure when communicating with Deaf family members. | Consider the linguistic structure of KSL rather than relying only on word-by-word translation. |
| Learning Resources | The participant considers available learning resources insufficient and supports broader online accessibility. | Provide accessible digital learning materials. |
| Order of Topics | The participant recommended learning letters first, followed by family vocabulary, colours, and workplaces. | Organize lessons progressively from fingerspelling to everyday topics. |
| Practice and Retention | The participant reported forgetting signs after a long period without regular communication. | Support repetition and regular practice. |
| Video Format | The participant recommended including spoken meanings and text descriptions in instructional videos. | Include voice-over and readable text descriptions. |
| Exercises | The participant suggested identifying signs from videos and checking learners' own signing. | Include multiple-choice quizzes and investigate optional camera-based verification. |
| Motivation | The participant learned sign language primarily to communicate with family members. | Prioritize practical vocabulary and real-life communication scenarios. |

### 2.3 Implications for Application Design

The interview findings suggest several important design considerations.

**Video-Based Instruction**

Video demonstrations should be prioritized because they provide a clearer representation of movement than static pictures.

**Progressive Learning Structure**

The learning process should begin with fingerspelling and basic vocabulary before introducing more complex signs and expressions.

**Regular Practice**

Interactive exercises and opportunities to review previously learned material should support continued practice.

**Feedback Mechanisms**

The application should provide feedback through quizzes. Camera-based gesture verification may be investigated as an optional extension.

**Accessible Learning Content**

Instructional videos should include clear text descriptions and, where appropriate, voice-over explanations.

### 2.4 Interview Limitations

The interview involved only one participant who has personal experience communicating with Deaf family members but is not a certified sign language interpreter or teacher.

Therefore, the findings provide qualitative insights into individual learning experiences rather than representative conclusions about all KSL learners.

The results should be considered alongside the survey findings presented in Section 12.

---

## 3. Survey Results

### 3.1 Survey Overview

A bilingual Google Forms survey was conducted on **21–22 October 2026** to identify potential users' experiences, learning preferences, and expectations regarding a mobile application for Kazakh Sign Language.

The questionnaire consisted of **15 questions** and received **19 responses**.

### 3.2 Respondent Characteristics

The survey participants belonged to the following age groups:

| Age Group | Number of Respondents |
|---|---:|
| Under 18 | 2 |
| 18–21 | 14 |
| 22–25 | 3 |
| **Total** | **19** |

Participants reported the following motivations or backgrounds:

| Background | Respondents |
|---|---:|
| General interest or curiosity | 16 |
| Deaf or hard-of-hearing relative, friend, or colleague | 2 |
| Studying or planning to become a sign language interpreter | 1 |

Most respondents had little or no experience with sign language.

| Sign Language Knowledge | Respondents |
|---|---:|
| No knowledge | 16 |
| Know individual signs | 2 |
| Can hold a simple conversation | 1 |

### 3.3 Interest in a Mobile Learning Application

Participants rated their interest in using a KSL learning application on a five-point scale.

| Interest Rating | Respondents |
|---|---:|
| 5 — Very Interested | 9 |
| 4 | 5 |
| 3 | 1 |
| 2 | 1 |
| 1 — Not Interested | 3 |
| **Total** | **19** |

The average interest rating was approximately **3.8 out of 5**.

Overall, **14 out of 19 respondents** rated their interest as 4 or 5.

These findings suggest interest in a beginner-oriented mobile learning application among the surveyed participants.

### 3.4 Barriers to Learning KSL

Participants identified several barriers that prevent them from learning Kazakh Sign Language.

| Barrier | Respondents |
|---|---:|
| Lack of time | 10 |
| Limited KSL learning materials | 4 |
| Lack of accessible courses nearby | 4 |
| Other reasons | 1 |

The most frequently reported barrier was a lack of time.

This finding supports considering short, flexible learning activities that users can complete independently.

No respondent reported previous experience using a dedicated sign language learning application.

Seven respondents mentioned communication with signers, while six mentioned YouTube or mobile applications as learning methods they had used or would consider.

### 3.5 Preferred Learning Formats

Respondents were asked which learning formats they would prefer.

| Learning Format | Respondents |
|---|---:|
| Short video lessons | 16 |
| Tests and exercises | 12 |
| Game-based tasks | 12 |
| 3D avatars or animations | 8 |
| Pictures with descriptions | 8 |
| Live online lessons with a teacher | 7 |
| Videos with subtitles | 6 |

Short video lessons were the most frequently selected format.

Interactive tests and game-based tasks were also popular among respondents.

These findings support the proposed combination of video instruction and interactive exercises in margau-YM.

### 3.6 Preferred Application Features

Participants identified the features they considered useful in a KSL learning application.

| Feature | Respondents |
|---|---:|
| Camera-based gesture verification | 13 |
| Interactive tests | 11 |
| Thematic learning categories | 10 |
| Searchable sign dictionary | 9 |
| Progress tracking | 8 |
| Reminders and learning streaks | 7 |
| Gamification elements | 7 |

Camera-based gesture verification received the highest number of selections.

However, because this feature requires additional technical development and validation, it is considered optional for the initial MVP.

The core application will prioritize thematic lessons, video demonstrations, interactive quizzes, and progress tracking.

### 3.7 Preferred Learning Topics

Respondents identified several topics they would like to study first.

The most frequently selected topics were:

1. **Greetings and Introductions:** Approximately 16 respondents.
2. **Alphabet and Numbers:** Approximately 12 respondents.
3. **Family:** Approximately 10 respondents.
4. **Health and Food:** Approximately 5 respondents each.

These preferences will inform the initial organization of learning categories.

### 3.8 Payment Preferences and Undesirable Features

Survey responses showed different attitudes toward paying for a KSL learning application.

| Payment Preference | Respondents |
|---|---:|
| Willing to pay | 9 |
| Depends on application quality | 5 |
| Prefer a free application | 5 |

Among the nine respondents willing to pay, seven preferred a small monthly payment, while two preferred a one-time payment.

Five respondents specifically mentioned that the application should avoid intrusive advertisements.

One respondent emphasized that the application should not be expensive.

### 3.9 Additional User Suggestions

Open-ended responses included several suggestions for improving the proposed application:

- A simple and understandable interface.
- Accessibility and inclusiveness.
- Opportunities to practice with other people.
- A wider variety of learning materials.
- Community-based learning features.
- Support for additional sign languages in the future.

These suggestions will be considered during later development stages according to project priorities and available resources.

### 3.10 Survey Limitations

The survey involved a small convenience sample of 19 respondents, most of whom were between 18 and 21 years old.

Only three respondents reported a relevant personal connection to Deaf individuals or sign language interpreting.

Consequently, the findings primarily reflect the preferences of hearing beginners and cannot be generalized to the wider Deaf community or all potential KSL learners.

Further user testing and consultation with knowledgeable signers will be important during application development.

---

## 4. Summary of User Research Findings

The interview and survey provide preliminary evidence supporting the proposed direction of margau-YM.

The main findings are:

1. **Video-based learning is a priority.** Both the interview participant and most survey respondents preferred video demonstrations for learning signs.
2. **Structured learning is important.** The interview suggested beginning with fingerspelling and basic vocabulary, while the survey highlighted interest in greetings, numbers, and family-related topics.
3. **Interactive practice is valuable.** Respondents expressed interest in quizzes, game-based exercises, and opportunities to repeat learned material.
4. **Camera-based verification is desirable but technically challenging.** It was the most frequently requested feature, but its implementation requires additional feasibility assessment.
5. **Accessibility and simplicity should guide design decisions.** Participants emphasized clear explanations, convenient navigation, and accessible learning materials.

These findings inform the functional requirements and preliminary interface design of margau-YM.

The research results will be used as initial design evidence rather than definitive proof of the application's effectiveness.

