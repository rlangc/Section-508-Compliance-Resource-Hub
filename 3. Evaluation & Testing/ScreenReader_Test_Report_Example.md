# Screen Reader Test Report – Example

## Project Title
"Cybersecurity Awareness Training – Module 1: Email Threats"

## Date of Test
June 14, 2025

## Tester Information
- **Name:** Jordan Ellis  
- **Role:** Accessibility Specialist  
- **Assistive Technology Used:** NVDA (NonVisual Desktop Access) v2024.1  
- **Browser/Platform:** Google Chrome 125.0.6422.61 on Windows 11

---

## 1. Objective

To assess the screen reader compatibility and navigational accessibility of Module 1 using NVDA. The test aims to determine whether users relying on assistive technology can successfully understand, navigate, and interact with all core learning elements.

---

## 2. Content Tested

| Content Area                  | Type                        | Format         |
|------------------------------|-----------------------------|----------------|
| Welcome Screen               | Instructional Text          | Slide (Storyline) |
| Interactive Knowledge Check  | Multiple Choice Quiz        | HTML5          |
| Embedded Video               | Captioned Instructional Video | MP4 (embedded) |
| Job Aid Download             | Linked PDF                  | External Link  |

---

## 3. Test Results Summary

| Criteria                                | Result     | Notes                                                                 |
|----------------------------------------|------------|-----------------------------------------------------------------------|
| Screen reader reads page title         | ✅ Pass    | Title is announced correctly on module load                           |
| Logical reading order                   | ✅ Pass    | Content read in correct visual order; tab sequence aligns with design |
| Alt text present for images             | ⚠️ Partial | 1 decorative image announced unnecessarily; no `aria-hidden="true"`   |
| Form fields (quiz) labeled              | ✅ Pass    | All radio buttons and questions read aloud with context               |
| Video controls accessible               | ✅ Pass    | Keyboard and screen reader both navigate native video player          |
| Captions and transcript available       | ✅ Pass    | Closed captions provided; transcript accessible via adjacent button   |
| Navigation buttons (Next/Back) labeled  | ⚠️ Partial | “Button 1” announced instead of “Next”; ARIA labels missing           |
| Downloadable resource clearly labeled   | ✅ Pass    | Link to job aid PDF announced correctly                               |

---

## 4. Detailed Observations

### 🔹 Welcome Screen
- NVDA reads: “Welcome to Module 1: Email Threats.”
- All heading levels (H1–H3) are correctly recognized.
- Alt text: “Shield icon” is read; recommend marking as decorative.

### 🔹 Interactive Quiz
- Question: “Which of the following is an example of phishing?”
- All choices are read aloud with role and selection status.
- Keyboard navigation allows full participation.
- Focus returns properly after selection.

### 🔹 Video Player
- Play/pause buttons are announced and operable via keyboard.
- Transcript button is read as “Transcript – opens in pop-up.”

### 🔹 Navigation Controls
- Issue: NVDA announces buttons as “Button 1”, “Button 2.”
- Suggested Fix: Add meaningful ARIA labels (`aria-label="Next Slide"`).

---

## 5. Recommendations

- Apply `aria-hidden="true"` to decorative images.
- Add ARIA labels or screen-reader friendly text to navigation buttons.
- Review contrast of focus outlines during keyboard tabbing for visibility.

---

## 6. Conclusion

The module is generally screen reader compatible, with all key learning elements accessible through NVDA. Minor improvements are recommended to optimize the screen reader experience and fully meet Section 508 and WCAG 2.1 standards.

---

## 7. Attachments

- `Screenshot_Focus_Issue_NavButtons.png`
- `Accessibility_Audit_Log_Module1.xlsx`
- `Transcript_Module1.pdf`

---

> ✅ Final Verdict: **Pass with Minor Remediation**
