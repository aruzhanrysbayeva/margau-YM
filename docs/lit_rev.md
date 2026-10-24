
# margau-YM — Literature Review and Research Gap

**Diploma Project:** Deployment of Mobile Application on Interactive E-Learning Platform for Kazakh Sign Language (KSL)

**Project Stage:** First Pre-Defense  
**Date:** October 24, 2026

---

## 1. Literature Review

This review covers twelve sources (journal papers and conference papers, 2021–2026). They are grouped into four themes: mobile and gamified sign language learning, digital learning technologies, Kazakh Sign Language resources, and sign language recognition.

The structured comparison matrix includes the research problem, methods, datasets, technologies, evaluation metrics, main findings, and limitations of each publication.

### 1.1 Mobile and Gamified Applications for Sign Language Learning

Several studies have developed mobile applications for learning sign languages.

Cabanillas-Carbonell et al. (2022) developed an augmented reality application for Peruvian Sign Language using 3D hand models, learning modules, and challenges. In a pre-experimental study involving 30 adults, the learning score increased from 4.13 to 9.67, while the information score increased from 2.27 to 9.07. However, the study did not include a control group.

Mohammad et al. (2022) developed MySign, a gamified Android application for Arabic Sign Language that includes letters, numbers, thematic vocabulary, memory games, and multiple-choice quizzes. In an experiment involving 10 deaf children aged six, the application group achieved a post-training score of 8.2 compared with 6.9 in the control group (p = 0.010). However, the sample size was small, and the intervention lasted only one week.

Siong et al. (2021) designed SLEM, a Malaysian Sign Language application incorporating thematic categories, a dictionary, fingerspelling, practice questions, and daily streaks. The proposed system used Google Cloud AutoML Vision to check learners' signs from photographs.

Their survey of 44 respondents found that 95.5% expressed interest in the application, while 39.4% preferred video tutorials. A built-in dictionary was also frequently requested. However, the study primarily presented the application design and did not report evaluation results for the completed system or recognition accuracy.

Hendriarto et al. (2024) applied a Design Thinking approach to develop V-Voice, a mobile learning prototype incorporating animated videos, educational games, and lessons for deaf learners. The prototype received positive design evaluations from more than 60 respondents, but learning effectiveness was not quantitatively measured.

### 1.2 Digital Technologies for Language Learning

Sari et al. (2026) conducted a scoping review of 45 studies published between 2014 and 2024 on digital technologies supporting language learning among children with hearing impairment.

Mobile applications were the most common technological approach, appearing in 26 studies. Interactive visual tools were found to support vocabulary learning. However, only 12 studies reported efficacy outcomes, and evidence regarding broader sign language learning remained limited.

The authors also identified insufficient long-term evaluation and limited cultural adaptation.

Ishaq et al. (2021) systematically reviewed 67 studies on mobile-assisted and gamified language learning. Their findings indicated that language-specific learning theories, validated educational content, and personalized assessment were insufficiently addressed in several existing approaches.

Together, these studies suggest that mobile and gamified learning technologies offer promising opportunities for language education, while emphasizing the importance of instructional quality and systematic evaluation.

### 1.3 Kazakh Sign Language Resources and Language Technology

Recent research on Kazakh Sign Language has primarily focused on datasets, recognition methods, and translation technologies.

Mukushev et al. (2022) introduced FluentSigners-50, a Kazakh-Russian Sign Language dataset containing 43,250 videos of 173 sentences performed by 50 signers.

The research demonstrated challenges in generalizing recognition models to unfamiliar signers and unseen sentences. The reported Word Error Rate was 24.9 on the signer-independent split and 52.0 on unseen sentences.

Yerimbetova et al. (2025) developed a parallel corpus for Kazakh text and sign language glosses. Their experiments showed that a Transformer-based approach outperformed a Seq2Seq model for text-to-gloss translation, achieving BLEU scores of approximately 0.775 and 0.675, respectively.

Amangeldy et al. (2026) investigated multilingual transformer-based models for converting Kazakh text into sign language glosses. The study used 11,190 text–gloss pairs and reported a BLEU score of 90.12. However, the system produced gloss representations rather than validated instructional sign videos.

Mnuarbek et al. (2026) developed a speech-to-sign gesture translation prototype with approximately 1,200 gesture entries, most of which represented static signs. The system achieved 85.8% word accuracy and 70.5% sentence accuracy.

These studies contribute valuable linguistic resources and technical approaches. However, their primary objectives concern recognition, translation, and data processing rather than the development and evaluation of beginner-oriented mobile learning environments.

### 1.4 Sign Language Recognition as Learner Feedback

Tao et al. (2024) reviewed traditional and deep learning approaches to sign language recognition.

The review identified several challenges, including limited signer independence, computational requirements, and reduced performance on larger datasets. For example, the reported recognition accuracy on WLASL was 57.13% in one evaluated setting.

Kim and Kim (2024) investigated recognition performance under variable video frame rates in mobile environments.

At 5 frames per second, their dynamic sampling method achieved 77.37% top-1 accuracy compared with 10.83% using fixed sampling. However, the experiments were performed under simulated mobile conditions using server-side processing.

These findings indicate that camera-based sign recognition is technically feasible but requires careful evaluation across different users, devices, and recording conditions.

For margau-YM, gesture verification is therefore considered an optional feature initially limited to a small set of selected signs.

---

## 2. Research Gap and Project Contribution

The reviewed literature identifies several challenges relevant to the development of interactive Kazakh Sign Language learning applications.

### 2.1 Limited Evaluation of KSL Learning Applications

Existing digital platforms provide educational resources for Kazakh Sign Language. However, the reviewed scientific literature provides limited evidence regarding the usability and measurable learning outcomes of these specific applications.

Research on KSL has largely concentrated on recognition datasets, translation systems, and linguistic resources rather than evaluating complete educational learning experiences.

### 2.2 Limitations in Learning Effectiveness Evaluation

Several studies investigating sign language learning applications involved small participant samples, short interventions, or limited evaluation of educational outcomes.

For example, Mohammad et al. (2022) evaluated an application with 10 children over one week, while Siong et al. (2021) primarily presented system design without evaluating the completed application.

These limitations highlight the importance of incorporating measurable evaluation methods into future educational applications.

### 2.3 Challenges in Gesture Recognition

Automatic sign recognition can provide useful feedback, but existing research identifies challenges related to signer variability, recording conditions, device performance, and model generalization.

These challenges must be considered when designing reliable feedback mechanisms for beginner learners.

### 2.4 Integration of Language Technology and Educational Design

Research on KSL translation and recognition has produced valuable technical resources.

However, implementing language technology within an educational application requires additional considerations, including curriculum organization, learner interaction, instructional feedback, and usability.

### 2.5 Need for Structured and User-Centered Learning Experiences

Mobile learning research highlights the potential benefits of structured lessons, gamification, and interactive practice.

However, these features must be adapted to the visual and linguistic characteristics of sign language learning and evaluated with the intended users.

### 2.6 Contribution of margau-YM

margau-YM aims to address these challenges by designing, implementing, deploying, and evaluating an integrated mobile e-learning environment for beginner-level Kazakh Sign Language.

The proposed application combines:

- Progressive thematic learning paths.
- Video-based sign demonstrations.
- Interactive quizzes and immediate feedback.
- Learning progress tracking.
- Mascot-supported user interaction.
- Accessible and beginner-oriented interface design.
- Optional camera-based gesture verification.

The project's contribution lies in the engineering implementation and user-centered evaluation of a coherent learning experience that integrates educational content, practice, feedback, and progress monitoring.

Rather than evaluating individual features in isolation, margau-YM will investigate how these components can work together to support independent KSL learning.

---

## 3. Literature Review Matrix

The complete Literature Review Matrix contains 12 publications and compares their research problems, methodologies, datasets, technologies, evaluation metrics, findings, and limitations.

**[View Literature Review Matrix](https://docs.google.com/spreadsheets/d/1iKdTMzmX3oBrsnwgXhiRMJ7QG0DWyhLJ-nKCjRXjZGM/edit?usp=sharing)**

---

## 4. References

Amangeldy, N., Yerimbetova, A., Tursynova, N., Gazizova, N., Dospol, N., & Orymbetov, A. (2026). Automatic transformation of Kazakh text into sign language glosses using multilingual transformer-based models. *Frontiers in Artificial Intelligence, 9*, Article 1867966. https://doi.org/10.3389/frai.2026.1867966

Cabanillas-Carbonell, M., Cusi-Ruiz, P., Prudencio-Galvez, D., & Herrera Salazar, J. L. (2022). Mobile application with augmented reality to improve the process of learning sign language. *International Journal of Interactive Mobile Technologies, 16*(11), 51–64. https://doi.org/10.3991/ijim.v16i11.29717

Hendriarto, H. A. M., Kusumawati, Y. A., & Arindiono, R. Y. (2024). The development of mobile application for the deaf to learn better. *Procedia Computer Science, 245*, 1225–1237. https://doi.org/10.1016/j.procs.2024.10.352

Ishaq, K., Mat Zin, N. A., Rosdi, F., Jehanghir, M., Ishaq, S., & Abid, A. (2021). Mobile-assisted and gamification-based language learning: A systematic literature review. *PeerJ Computer Science, 7*, Article e496. https://doi.org/10.7717/peerj-cs.496

Kim, T., & Kim, B. (2024). Techniques for detecting the start and end points of sign language utterances to enhance recognition performance in mobile environments. *Applied Sciences, 14*(20), Article 9199. https://doi.org/10.3390/app14209199

Mnuarbek, A., Bekarystankyzy, A., Turdalyuly, M., Oralbekova, D., & Dyussemkhanov, A. (2026). Speech-to-sign gesture translation for Kazakh: Dataset and sign gesture translation system. *Computers, 15*(3), Article 188. https://doi.org/10.3390/computers15030188

Mohammad, H., Tamimi, H., & Abu-Amara, F. (2022). An educational Arabic sign language mobile application for children with hearing impairment. *International Journal of Interactive Mobile Technologies, 16*(20), 114–129. https://doi.org/10.3991/ijim.v16i20.32427

Mukushev, M., Ubingazhibov, A., Kydyrbekova, A., Imashev, A., Kimmelman, V., & Sandygulova, A. (2022). FluentSigners-50: A signer independent benchmark dataset for sign language processing. *PLOS ONE, 17*(9), Article e0273649. https://doi.org/10.1371/journal.pone.0273649

Sari, A. D., Al Mahmud, A., Octavia, J. R., & Tyagi, S. (2026). Digital technologies for children with hearing impairments to support language learning: Scoping review. *JMIR Rehabilitation and Assistive Technologies, 13*, Article e85066. https://doi.org/10.2196/85066

Siong, T. J., Nasir, N. R. M., & Salleh, F. H. M. (2021). A mobile learning application for Malaysian sign language education. *Journal of Physics: Conference Series, 1860*, Article 012004.

Tao, T., Zhao, Y., Liu, T., & Zhu, J. (2024). Sign language recognition: A comprehensive review of traditional and deep learning approaches, datasets, and challenges. *IEEE Access, 12*, 75034–75060. https://doi.org/10.1109/ACCESS.2024.3398806

Yerimbetova, A., Sakenov, B., Sambetbayeva, M., Daiyrbayeva, E., Berzhanova, U., & Othman, M. (2025). Creating a parallel corpus for the Kazakh sign language and learning. *Applied Sciences, 15*(5), Article 2808. https://doi.org/10.3390/app15052808
