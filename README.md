# Science Quiz Online Platform - QA & Testing Portfolio
**University of Waikato | Trimester B, 2025**

## Project Overview
This cloud-based science quiz platform was built with a **Vue.js** frontend and **Python REST APIs**, deployed on **AWS**. As the **QA Engineer**, I ensured the platform's stability, security, and performance.

## Cloud Architecture
The system utilizes a modern AWS stack for high availability and security. I monitored application performance and logs using **Amazon CloudWatch** and assisted with the **DynamoDB** database transition.

(Cloud Architecture.png)

* **Compute:** EC2 with Load Balancing.
* **Storage & CDN:** S3 for static assets and CloudFront for global delivery.
* **Database:** DynamoDB for scalable data storage.
* **Security:** AWS Secrets Manager for credential protection.

---

## Testing & Verification
A comprehensive manual testing session was conducted to verify the functionality of the Science Quiz Platform across core workflows including user authentication, quiz participation, scoring, and data visualization. 

**In total, 19 test cases were executed.**

(Test Cases.png)

### Test Results Summary:
* **12 Passed:** Core features functioned as expected.
* **7 Inconclusive:** Minor issues or missing clarifications were observed, most of which have since been addressed through API updates.
* **1 Failed:** Question filtering by difficulty did not operate correctly during initial testing.

### Key Success Areas:
* **User Accounts & Security:**
    * Users can successfully register, log in, and log out.
    * Weak passwords are consistently rejected, enforcing strong password policies.
    * Password reset and change features work correctly, protecting account integrity.
* **Quiz Functionality:**
    * Quizzes load quickly, and questions display correctly.
    * Navigation between questions is smooth and intuitive.
    * The scoring system works reliably, highlighting incorrect answers.
    * The timer auto-submit feature ensures fair and consistent quiz completion.
* **Data Tracking:**
    * Quiz history is recorded accurately and displayed in the user profile.
    * Profile information updates correctly.

### Security Verification:
* **Password Strength Enforcement:** Accounts with weak credentials (e.g., "password123") were rejected, confirming robust password policies.
* **Login Protection:** The system correctly blocked repeated invalid login attempts. While no temporary lockout mechanism was implemented, this was a calculated balance between usability and security for this iteration.

## Conclusion
The testing confirmed that the platform’s authentication, quiz operations, and data tracking features work reliably. While some refinements remain (notably question filtering and mobile responsiveness gaps), the system is stable, secure, and ready for use.
