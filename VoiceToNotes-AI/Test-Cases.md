# Test Cases

This document contains the manual functional test cases prepared for the **VoiceToNotes.ai QA Technical Assessment**. 

The test cases cover the application's primary workflows, including landing page navigation, authentication, voice-to-text functionality, note management, AI-powered enhancements, negative scenarios, and account-related features. 

The objective is to validate the application's functionality, usability, and reliability while identifying potential defects through structured manual testing.


## Objective

The objective of these test cases is to verify that the core functionalities of VoiceToNotes.ai operate as expected under normal and edge-case scenarios. 

These test cases also ensure that critical user workflows remain stable and deliver a consistent user experience.

# 1. Landing Page & Navigation

<img width="1920" height="929" alt="screenshot-showing-the-login-page-of-voicetonotes-ai-web-app-page" src="https://github.com/user-attachments/assets/583b5d31-9936-4aba-99f0-9a9e6f6bddda" />


| Test ID | Preconditions         | Steps                                                  | Expected Result                 | Priority |
| ------- | --------------------- | ------------------------------------------------------ | ------------------------------- | -------- |
| TC-001  | Website is accessible | Open the landing page                                  | Landing page loads successfully | High     |
| TC-002  | Landing page loaded   | Navigate through Home, Features, Pricing, FAQ and Blog | All pages open successfully     | High     |
| TC-003  | Landing page loaded   | Click **Log In** and **Get Mobile App** buttons        | Correct destination page opens  | High     |

# 2. Authentication & Session Management

<img width="1920" height="929" alt="screenshot-showing-the-authentication-and-user-management-page-of-voicetonotes-ai" src="https://github.com/user-attachments/assets/b607cafa-9bcc-4997-a348-64f81e5718b6" />


| Test ID | Preconditions      | Steps                                                            | Expected Result                                  | Priority |
| ------- | ------------------ | ---------------------------------------------------------------- | ------------------------------------------------ | -------- |
| TC-004  | Valid user account | Login using valid credentials                                    | User is successfully authenticated               | Critical |
| TC-005  | Login page         | Enter invalid login credentials                                  | Appropriate validation message is displayed      | High     |
| TC-006  | User logged in     | Logout and attempt to access dashboard using browser back button | Protected pages remain inaccessible after logout | High     |


# 3. Voice-to-Text Workflow

<img width="1920" height="929" alt="screenshot-of-voicetonotes-ai-voice-to-text-overflow-page-insights" src="https://github.com/user-attachments/assets/257d34bd-b0dc-4668-98a1-73e5e3724d2c" />


| Test ID | Preconditions             | Steps                       | Expected Result                           | Priority |
| ------- | ------------------------- | --------------------------- | ----------------------------------------- | -------- |
| TC-007  | User logged in            | Grant microphone permission | Microphone access is enabled successfully | Critical |
| TC-008  | Microphone enabled        | Record a voice note         | Recording starts and stops successfully   | Critical |
| TC-009  | Voice recording available | Generate transcription      | Accurate transcription is displayed       | Critical |
| TC-010  | Transcription available   | Edit the generated text     | Edited content is updated successfully    | High     |
| TC-011  | Edited transcription      | Save the note               | Note is saved successfully                | High     |


# 4. Note Management

<img width="1920" height="929" alt="screenshot-of-voicetonotes-ai-web-page-showing-the -notes-management-section" src="https://github.com/user-attachments/assets/61870522-a2aa-4a12-a5d8-50c4f79f03f4" />


| Test ID | Preconditions           | Steps                   | Expected Result                | Priority |
| ------- | ----------------------- | ----------------------- | ------------------------------ | -------- |
| TC-012  | Existing note available | Search for a saved note | Relevant note is displayed     | Medium   |
| TC-013  | Existing note           | Edit note content       | Changes are saved successfully | Medium   |
| TC-014  | Existing note           | Delete the note         | Note is removed successfully   | High     |


# 5. AI Enhancements

<img width="1920" height="929" alt="voicetonotes-ai-web-page-section-showing-ai-generated-novels-and-saved-transcriptions" src="https://github.com/user-attachments/assets/af238282-454b-4256-8303-237bf447608e" />


| Test ID | Preconditions                  | Steps                             | Expected Result                             | Priority |
| ------- | ------------------------------ | --------------------------------- | ------------------------------------------- | -------- |
| TC-015  | Saved transcription            | Apply AI Enhance or Grammar Check | Improved content is generated successfully  | Medium   |
| TC-016  | AI-generated content available | Perform Undo and Redo actions     | Changes are reverted and restored correctly | Medium   |


# 6. Negative & Edge Case Testing

<img width="1920" height="929" alt="screenshot-of-voicetonotes-ai-web-page-showing-ai-assistance-in-note-making" src="https://github.com/user-attachments/assets/8b645310-1f1d-4e63-9eec-bb4ba7c070c3" />


| Test ID | Preconditions                          | Steps                              | Expected Result                                   | Priority |
| ------- | -------------------------------------- | ---------------------------------- | ------------------------------------------------- | -------- |
| TC-017  | Microphone permission prompt displayed | Deny microphone permission         | Appropriate permission error message is displayed | High     |
| TC-018  | Audio upload feature available         | Upload an unsupported audio format | File validation error message is displayed        | Medium   |


# 7. Support & Account

<img width="1920" height="929" alt="settings-and-account-section-in-voicetonotes-ai-webpage" src="https://github.com/user-attachments/assets/79513796-dd6e-492f-b39e-ff486ad88993" />


| Test ID | Preconditions          | Steps                                       | Expected Result                 | Priority |
| ------- | ---------------------- | ------------------------------------------- | ------------------------------- | -------- |
| TC-019  | User logged in         | Open Profile or Account Settings            | Profile page loads successfully | Medium   |
| TC-020  | Contact form available | Submit the contact form using valid details | Form is submitted successfully  | Medium   |

# 8. Mobile Responsive Testing

<img width="1080" height="2400" alt="mobile-chrome-browser-screenshot-of-voicetonotes-ai-web-page-shoing-error" src="https://github.com/user-attachments/assets/137aed86-c032-4799-ab01-c373c67e8072" />


| Test ID | Preconditions | Steps | Expected Result | Priority |
|---------|---------------|-------|-----------------|----------|
| TC-021 | Website accessible on a mobile device | Open the landing page on a mobile browser | Landing page loads correctly without layout issues | High |
| TC-022 | Mobile landing page loaded | Navigate through Home, Features, Pricing, FAQ, and Blog | All navigation links function correctly and pages are responsive | High |
| TC-023 | Mobile landing page loaded | Tap the **Log In** and **Get Mobile App** buttons | Appropriate pages or actions are triggered successfully | High |
| TC-024 | Mobile dashboard accessible | Verify UI elements such as buttons, menus, forms, and text fields | All interface elements are properly aligned, visible, and usable | High |
| TC-025 | Mobile application in use | Rotate the device between portrait and landscape orientations | The layout adapts correctly without breaking the user interface | Medium |

# Conclusion

The above test cases provide structured coverage of the primary functional areas of VoiceToNotes.ai, including navigation, authentication, voice transcription, note management, AI features, edge-case scenarios, and account management. 

These test cases serve as a foundation for validating application quality, ensuring feature reliability, and identifying defects before deployment.
