# KSL-4: Existing Systems and Technology Comparison

Project: margau-YM, a mobile application on an interactive e-learning platform for Kazakh Sign Language (KSL)

## 1. Existing System Comparison

Three complementary systems were selected: Duolingo, AI-Ym and Lingvano.

- **Duolingo** is a design benchmark for gamified language learning rather than a direct KSL competitor. Its short lessons, structured learning path, progress indicators and Duo mascot inform the design of practice and feedback.
- **AI-Ym** is a direct KSL-domain comparison.
- **Lingvano** is a specialized sign-language learning reference, including video-based teaching and a mascot named Mano.

Together, these systems allow comparison of general learning design, local language coverage and sign-language-specific interactions.

The matrix distinguishes documented or observed features from unverified claims. AI-Ym gesture recognition produced an error in one exploratory attempt reported by the project team; this does not establish a general service failure. Features of margau-YM are proposed, not yet implemented.

| Criterion | Duolingo | AI-Ym | Lingvano |
| --- | --- | --- | --- |
| Learning domain | Spoken/written languages | KSL | Selected sign languages (not KSL) |
| Video sign demonstrations | Not core | Yes | Yes |
| Structured learning | Yes | Yes | Yes |
| Interactive practice | Yes | Yes | Yes |
| Progress tracking | Yes | Yes | Yes |
| Streaks / series | Yes | Yes (team observation) | Yes |
| Mascot | Duo | Not observed | Mano |
| Gesture checking | Not sign-specific | Advertised; error in one test | Available (team observation) |
| Dictionary | No dedicated sign dictionary | Available | Available |
| Gamification | Extensive | Available | Available |

**Comparative interpretation.** AI-Ym establishes that KSL learning tools already exist. Duolingo provides an interaction-design reference; Lingvano provides sign-language-specific teaching patterns. margau-YM will be differentiated through its deliberately scoped beginner curriculum, locally validated video content, integrated learning flow and evaluation with intended users. These are design priorities and planned contributions, not claims that competing products lack the same features.

## 2. Technology Comparison and Selection

Technology alternatives were evaluated against the team's JavaScript/Node.js experience, support for iOS and Android, integration effort, maintainability and feasibility within a two-person project. The following selections are preliminary architectural decisions, not implemented components.

### 2.1 Mobile framework

| Criterion | React Native + Expo | Flutter | Native Android |
| --- | --- | --- | --- |
| Language | JavaScript / TypeScript | Dart | Kotlin / Java |
| Team familiarity | High | Low | Moderate |
| Platform support | iOS + Android | iOS + Android | Android only |
| Video and camera | Supported | Supported | Supported |
| MVP fit | High | Moderate | High if Android-only |

**Proposed: React Native + Expo.** It leverages existing JavaScript knowledge and supports both target platforms without introducing Dart.

### 2.2 Backend and data

| Criterion | Supabase | Firebase | Node.js + PostgreSQL |
| --- | --- | --- | --- |
| Data model | PostgreSQL relational | Firestore document | PostgreSQL relational |
| Auth and API | Managed | Managed | Custom development |
| Operational effort | Low–moderate | Low–moderate | Higher |
| Lesson / quiz relations | Natural SQL fit | Requires document modeling | Natural SQL fit |
| MVP fit | High | High | Moderate |

**Proposed: Supabase.** Relational data suits topics, lessons, questions and learner progress; managed services reduce custom server work. Node.js remains an option if custom logic becomes necessary.

### 2.3 Video storage

| Criterion | Supabase Storage | Firebase Storage | Cloudinary |
| --- | --- | --- | --- |
| Video files | Supported | Supported | Supported |
| Integration | Same Supabase ecosystem | Same Firebase ecosystem | Separate media service |
| Access control | Storage policies | Security rules | Media access configuration |
| Media transformations | Additional work may be needed | Additional work may be needed | Specialized tools |
| MVP fit | High with Supabase | High with Firebase | High for media-heavy needs |

**Proposed: Supabase Storage**, to keep video metadata and access management close to the selected data platform. File sizes, streaming behavior and costs require validation.

### 2.4 Optional gesture verification

Python and MediaPipe may be evaluated for landmark extraction, but landmark detection alone does not establish correctness of KSL signs. Reliable feedback would require a defined vocabulary, suitable labeled examples, validation across signers and a measurable accuracy threshold. This module is excluded from the mandatory MVP.
