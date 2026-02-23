# Hirechannel Hirevoice Assessment

Welcome to the Hirechannel technical assessment! This challenge is designed to evaluate your fullstack development skills, with a focus on video handling and system integration capabilities.

Should you have any doubts, feedback or questions, please don't hesitate to contact alvaro@hirechannel.com.

Please, read the whole document before starting the assessment.

## ⚠️ Disclaimer
- This is a paid assessment with a compensation of a 150€ Amazon gift card to be sent after the assessment is submitted
- This technical assessment is solely for evaluation purposes
- Participation does not imply or guarantee any employment relationship
- The results of this assessment will not be used internally.
- The results will not be used for any other purposes under any circumstances

After reading the document and prior to starting the assessment, you must send an email to alvaro@Hirevoice.com confirming your acceptance of the terms above:

```
Subject: Hirevoice Technical Assessment Acceptance

Hello,

I accept the terms and conditions of the Hirevoice technical assessment.

The terms and conditions are:

- This is a paid assessment with a compensation of a 150€ Amazon gift card to be sent after the assessment is submitted
- This technical assessment is solely for evaluation purposes
- Participation does not imply or guarantee any employment relationship
- The results of this assessment will not be used internally by Hirechannel
- The results will not be used for any other purposes under any circumstances

Best regards,

[Your Name]
```

## Table of Contents
- [Objective](#-objective)
- [Key Requirements](#-key-requirements)
  - [Frontend](#frontend-estimated-15-2h)
  - [Backend](#backend-estimated-15-2h)
- [Technical Guidelines](#-technical-guidelines)
- [Bonus Features (Optional)](#-bonus-features-optional)
- [Submission Requirements](#-submission-requirements)
- [Time Expectation](#️-time-expectation)
- [Evaluation Criteria](#-evaluation-criteria)
- [Getting Started](#-getting-started)
- [Consideraciones Importantes](#️-consideraciones-importantes)
- [Notes](#-notes)

## 🎯 Objective

Build a simplified version of a video interview system where candidates can record their answers to a predefined question, and the system processes and evaluates the recording automatically using AI.

## 🔑 Key Requirements

### Frontend
- Build a single-page application using React.
- Feel free to use any libraries you want.
- Allow candidates to record video answers (max 60 seconds) for up to 5 questions of your choice. Some examples could be: 
**“Tell us about yourself”**
**“What’s your greatest achievement?”**
**“Where do you see yourself in 5 years?”**
**“Why do you want to work with us?”** 
**“How do you handle working under pressure?”**

- Essential features:
  - Camera/microphone permission handling.
  - Start/stop recording controls.
  - A clean, simple UI (no authentication required).
  - A timer: once the candidate starts recording, the timer should start. Once the timer reaches 0, the recording should stop and go to the next question.

### Backend
Build a backend using the technologies you prefer with a key integration to process the recording:
- **AI Evaluation System**
   - Transcribe the recorded video using a Speech-to-Text API.
   - Send the transcription to an LLM to evaluate the candidate's answer.
   - Retrieve an evaluation score (from 1 to 5) for the candidate's answer. You don't need to display the score in the frontend. Just print it to the console in the server. The evaluation criteria is up to you.
   - Process these steps independently and asynchronously from the main recording flow.
   - As part of your solution, please include the exact prompt you used to evaluate the candidate's answer using the LLM

Note: We will provide an OpenAI API key for you to use in this assessment.

The solution must be extensible and loosely coupled with the answer submission flow.

## 💡 Technical Guidelines

- **Architecture**: Use the technologies you prefer. Design your solution for easy extensibility.
- **Async Processing**: Keep the main flow responsive while processing
- **Browser Handling**:
  - Focus on compatibility with the latest versions of Chrome or any Chromium-based browser.
- **Error Handling**: Implement proper error handling throughout the application.

## 🎁 Bonus Features (Optional)

If you finish early, feel free to:
- add additional fun integrations or creative features. Anything you want!

Note: Only attempt these if you've completed all core requirements with time to spare.

## 📝 Submission Requirements

### Code Repository
- Please create a new repository using this repository as a template (click "Use this template" button) and add GitHub users `monterrubio12` and `inakin` as a collaborators.

### Screen Recording
Record your screen **only during the first 2 hours** of assessment-related tasks. If you are using multiple screens, please record all of them in a single video.

The recording should include:
- Your implementation process
- Any searches or documentation lookups, usage of resources, tools, or AI assistants
- Problem-solving activities related to this challenge

This recording helps us:
- Understand your workflow and problem-solving approach
- Validate the authenticity of your work
- Gain insight into your coding practices

*Note: Please only record activities directly related to this assessment. Make sure the recording quality is clear and readable. You can use any screen recording software you prefer.*

### AI Tools Documentation
Please include in your submission an explicit explanation of:
- Which AI tools you used during the assessment
- Why you chose those tools over other alternatives
- How you used them in your workflow
- How you provided feedback to the AI agents to achieve fast feedback loops

## ⏱️ Time Expectation

Approximately 4-5 hours.

### 🚨 Important Note

When you reach the 2 hours mark, please:
1. Stop recording your screen.
2. Record a brief video recording summarizing and providing context about what you did. Feel free to give any feedback or suggestions for the assessment.
3. Before continuing, send an email to alvaro@hirechannel.com letting us know you're done with the first 2 hours and send us the video recording of the first 2 hours and the summary video.
4. After that, you will have 24 hours to complete the assessment. No recording is needed for this step.
5. Once you're done, we will review your submission and get back to you for a follow-up video call.

**We value your time** and want to understand your thought process, even if not all features are completed. The follow-up discussion will give us insight into your problem-solving approach and technical vision for the complete solution. Your feedback on the time estimation will help us improve our assessment process.


## 🔍 Evaluation Criteria

| Area          | Key Points                                                       |
|---------------|------------------------------------------------------------------|
| **Frontend**  | Clean UI; robust media handling; effective error feedback        |
| **Backend**   | Thoughtful system design; well-implemented integrations          |
| **Code Quality** | Clean, maintainable, well-documented code                     |
| **Problem Solving** | Sound architecture decisions                               |
| **AI Fluency** | Effective use of AI tools and agents in the development workflow |

## 🚀 Getting Started

1. Create your own private repository using this repository as a template:
   - Click the green "Use this template" button at the top of this page
   - Select "Create a new repository"
   - Make sure to set it as "Private"
   - Create your repository
2. Add GitHub users `monterrubio12` and `inakin`as a collaborator to your new repository:
   - Go to Settings > Collaborators
   - Click "Add people"
   - Enter `monterrubio12`
   - Select "Add to repository"
   - Repeat for the rest of users
3. Implement the required features based on the guidelines above.
4. Submit your solution.

## ⚠️ Consideraciones Importantes

- Estamos creando una empresa de producto, por lo que en esta entrevista valoraremos tanto el sentido y gusto de producto como la robustez y estabilidad de la solución técnica.
- Recomendamos encarecidamente utilizar un agente para el desarrollo de la prueba.
- Buscamos gente que sea capaz de traer soluciones a problemas complejos y creemos que una parte de la resolución de este tipo de problemas va a consistir en escribir sobre ellos. Así que te pedimos que escribas un README lo más detallado que puedas.
- La experiencia del entrevistador es importante, por lo que cuanto más sencillo sea para nosotros probar lo que has desarrollado, más lo valoraremos.

## 📋 Notes

- **We encourage using AI tools** (Claude, Cursor, Windsurf, ChatGPT, etc.). Please use all the AI tools you're comfortable with and don't hide it. We are very interested in understanding how you use AI tools in your workflow.
- Even when using AI, we expect you to make your own engineering and technical decisions. We want to understand why you made those decisions and which alternatives you considered.
- Please tell us what you think about the tech stack proposed in this assessment and if you would use a different one and why.
- Focus on building a functional solution over a pixel-perfect UI.
- If you have any questions, feel free to ask.
- Don't worry about perfect code organization—we value working functionality over perfect architecture.

**Good luck!** 🎉
