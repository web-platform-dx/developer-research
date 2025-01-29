# Web App Short Survey

## Date
Survey run between 2024-08-05 - 2024-08-23 to 5% of MDN users.

## Questions

1. In the past year, have you built an installable web application? _(single selection)_
  * Yes
  * No
  * Don't know

2. In your experience, are web applications sufficiently capable to replace native apps on these platforms? _(each option listed with 6 choices: "Don't know", "Not at all capable", "Not very capable", "Somewhat capable", "Very capable", "Completely capable")_
  * Android
  * iOS
  * macOS
  * Windows

3. In your experience, what is the biggest challenge building web applications? _(free-form text)_

## Results

### Response Counts

*   Completion Rate: 99.9%
*   Complete: 752
*   Partial: 1
*   Totals: 753

### Q1 - In the past year, have you built an installable web application?

| Value       | Percent | Responses |
| ----------- | ------- | --------- |
| Yes         | 34.2%   | 257       |
| No          | 56.1%   | 421       |
| Don't know  | 9.7%    | 73        |
| Totals      |         | 751       |


### Q2 - In your experience, are web applications sufficiently capable to replace native apps on these platforms?

| Platform | Don't know | Not at all capable | Not very capable | Somewhat capable | Very capable | Completely capable | Responses |
| -------- | ---------- | ------------------ | ---------------- | ---------------- | ------------ | ------------------ | --------- |
| Android  | 46 (19.0%) | 15 (6.2%)          | 15 (6.2%)        | 69 (28.5%)       | 73 (30.2%)   | 24 (9.9%)          | 242       |
| iOS      | 50 (21.4%) | 32 (13.7%)         | 36 (15.4%)       | 68 (29.1%)       | 36 (15.4%)   | 12 (5.1%)          | 234       |
| macOS    | 62 (26.7%) | 22 (9.5%)          | 23 (9.9%)        | 56 (24.1%)       | 45 (19.4%)   | 24 (10.3%)         | 232       |
| Windows  | 39 (16.0%) | 17 (7.0%)          | 13 (5.3%)        | 58 (23.8%)       | 76 (31.1%)   | 41 (16.8%)         | 244       |
| Totals   |            |                    |                  |                  |              |                    | 244       |

### Q3 - In your experience, what is the biggest challenge building web applications? (free-form)
The following challenges were extracted from the free-form responses:
| Category                                      | Subcategory                                           | Count |
| :-------------------------------------------- | :---------------------------------------------------- | :---- |
| **Development & Technical Challenges**        | **Cross-Browser Compatibility & Standards**           | 34    |
|                                               | **API Limitations & Access to Native APIs**           | 27    |
|                                               | **UI/UX & Design**                                    | 19    |
|                                               | **Performance & Optimization**                        | 6     |
|                                               | **Frameworks, Tools, and Ecosystem**                  | 11    |
|                                               | **State Management & Data Persistance**               | 8     |
|                                               | **Service Workers & Offline Functionality**           | 4     |
| **User & Business Challenges**                | **Users expecting to get apps from an app store**     | 9     |
|                                               | **Development Process**                               | 5     |
| **Other & General Challenges**                | **Documentation & Learning Resources**                | 11    |
|                                               | **Security**                                          | 3     |
|                                               | **Uncategorized/Unclear**                             | 26    |
| **Totals**                                    |                                                       | 158   |

**Important Notes:**

*   **Multiple Categories:** Some responses touched upon multiple challenges and are therefore counted in more than one category. This is why the total count in the table is greater than the total number of free-form responses received.
*   **Relative Importance:** This table reflects the number of times a challenge was mentioned, not necessarily its importance to each respondent.



## Interpretation
This interpretation is provided by Kadir Topal of Google.


**Overall Sentiment:**

The responses to question 2 indicate a mixed sentiment regarding the capability of web applications to replace native apps across different platforms. While there's a degree of optimism, a significant portion of respondents expressed reservations about whether web apps are truly "sufficiently capable" replacements.

**Platform-Specific Breakdown:**

*   **Android:** Android received highly positive responses. A combined 68.6% (9.9% completely capable + 30.2% very capable + 28.5% somewhat capable) believe web apps are capable to some extent. This suggests that developers see Android as a relatively strong platform for web apps. However, 12.4% (6.2% not very capable + 6.2% not at all capable) still felt that web apps were not capable of replacing native apps and 19.0% selected don't know.
*   **Windows:** Windows showed an even higher level of confidence, with a combined 71.7% (16.8% completely capable + 31.1% very capable + 23.8% somewhat capable) of respondents indicating that web apps are capable to some extent. This might reflect the increasing adoption of web apps on Windows and the fact that the line between web and native is becoming blurred on desktop platforms. However, 12.3% (7.0% not very capable + 5.3% not at all capable) still felt that web apps were not capable of replacing native apps and 16.0% selected don't know.
*   **iOS:**  iOS has a lower confidence level compared to Android and Windows. While 49.6% (5.1% completely capable + 15.4% very capable + 29.1% somewhat capable) believe web apps are capable to some extent, a combined 29.1% (15.4% not very capable + 13.7% not at all capable) expressed that web apps are not capable, and 21.4% selected don't know. This aligns with the challenges mentioned in the free-form responses about restrictions and limitations on web technologies, particularly web apps, within the iOS ecosystem.
*   **macOS:** macOS received the highest percentage of "Don't know" responses (26.7%). This suggests uncertainty or perhaps less experience among respondents when it comes to building web apps specifically for macOS. While 53.8% (10.3% completely capable + 19.4% very capable +  24.1% somewhat capable) do feel that web apps are capable to some extent, 19.4% (9.9% not very capable + 9.5% not at all capable) expressed that web apps are not capable.

**Possible Reasons for Reservations:**

The free-form responses to Question 3 provide valuable context for these results. Developers cited challenges like:

*   **API Limitations:** Lack of access to certain native device features and APIs.
*   **Cross-Browser Compatibility:** Inconsistencies in browser implementations, especially with Safari on iOS.
*   **Performance:** Web apps sometimes struggle to match the performance of native apps.
*   **UI/UX Limitations:** Difficulty in achieving a truly native look and feel.
*   **User Perception:** Users are accustomed to install native apps from app stores and may be hesitant to adopt web apps.
