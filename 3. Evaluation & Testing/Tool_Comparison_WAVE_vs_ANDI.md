# Tool Comparison: WAVE vs. ANDI for 508 Accessibility Evaluation

## Purpose

This document provides a practical comparison of two widely used accessibility evaluation tools—**WAVE** (Web Accessibility Evaluation Tool) and **ANDI** (Accessible Name & Description Inspector). It is intended to support instructional designers, developers, and accessibility reviewers in selecting the most appropriate tool(s) when testing digital training content for Section 508 compliance.

---

## 1. Overview of Each Tool

### 🔹 WAVE (Web Accessibility Evaluation Tool)
- **Developer:** WebAIM
- **Access:** [https://wave.webaim.org](https://wave.webaim.org) or browser extension
- **Use Case:** Visual, summary-based accessibility reports; ideal for web-based learning modules and public-facing instructional content.

### 🔹 ANDI (Accessible Name & Description Inspector)
- **Developer:** U.S. Social Security Administration
- **Access:** [https://www.ssa.gov/accessibility/andi/help/install.html](https://www.ssa.gov/accessibility/andi/help/install.html)
- **Use Case:** In-depth testing of name, role, value, keyboard focus, and scripting; highly effective for interactive content, forms, and complex learning interfaces.

---

## 2. Comparison Table

| Feature / Capability                      | WAVE                              | ANDI                                  |
|------------------------------------------|-----------------------------------|----------------------------------------|
| **Developer**                            | WebAIM                            | U.S. Social Security Administration    |
| **Installation**                         | Chrome/Firefox extension or online| JavaScript bookmarklet (browser-based) |
| **508/WCAG Alignment**                   | WCAG 2.1 / Section 508            | WCAG 2.1 / Section 508                 |
| **Best for**                             | Public web content, LMS pages     | Web apps, interactive training, forms  |
| **Interface**                            | Visual report with icons and panels | Tab-based overlay UI                 |
| **Color Contrast Check**                 | Yes (pass/fail and ratios shown)  | Yes (live feedback and tooltips)       |
| **ARIA & Semantic Roles**                | Basic detection                   | Detailed breakdown                     |
| **Keyboard Focus Testing**               | Limited (requires manual follow-up)| Robust (Focus tab, tab order highlights)|
| **Form Field Validation**                | High-level                        | Deep-level (Label, Name, Description)  |
| **Error Flagging**                       | Summary with indicators           | Interactive walkthrough per element    |
| **Exportable Reports**                   | No (manual screenshot/export)     | No (manual logging only)               |
| **Learning Curve**                       | Beginner-friendly                 | Intermediate (requires familiarity)    |

---

## 3. Strengths & Use Cases

### ✅ WAVE – Strengths
- Fast, visual feedback for common web accessibility issues
- Color-coded interface with icons for headings, ARIA, alt text, etc.
- Useful for scanning static web-based training, syllabus pages, or documentation

**Ideal for:**
- Quick audits of LMS pages
- First-pass accessibility scans
- Designers new to accessibility testing

---

### ✅ ANDI – Strengths
- Excellent for interactive forms and dynamic content
- Highlights keyboard focus issues and improper labels
- Evaluates role, name, and description relationships thoroughly

**Ideal for:**
- Screen reader compatibility validation
- eLearning modules with custom navigation
- Detailed remediation assessments

---

## 4. Limitations

### ⚠️ WAVE
- Limited support for dynamic content or JavaScript-heavy training tools
- Can miss complex ARIA errors and keyboard focus problems
- Doesn’t evaluate scripts or advanced behaviors

### ⚠️ ANDI
- Not beginner-friendly; requires accessibility knowledge
- Doesn’t generate visual dashboards or downloadable reports
- Bookmarklet format may not work in locked-down enterprise environments

---

## 5. Recommendations

| Scenario                                         | Recommended Tool     |
|--------------------------------------------------|-----------------------|
| Static content (web pages, documentation)        | **WAVE**              |
| Interactive learning modules (quizzes, sliders)  | **ANDI**              |
| Testing keyboard navigation and tab order        | **ANDI**              |
| Quick scans for alt text, contrast, headings     | **WAVE**              |
| Form accessibility and ARIA validation           | **ANDI**              |
| Beginner-level evaluations                       | **WAVE**              |

---

## 6. Combined Workflow Suggestion

For optimal 508 evaluation coverage:
1. **Start with WAVE** for a broad overview and visual feedback.
2. **Follow with ANDI** to test deep accessibility of forms, interactions, and focus order.
3. **Use screen readers (e.g., NVDA)** to validate real-world usability.

---

## 7. Resources

- [WAVE Tool](https://wave.webaim.org)  
- [ANDI Tool](https://www.ssa.gov/accessibility/andi/help/install.html)  
- [W3C WCAG 2.1 Standards](https://www.w3.org/TR/WCAG21/)  
- [Section508.gov – Testing Tools](https://www.section508.gov/test/tools/)

---

> “No single tool can catch everything—accessibility is best ensured through layered evaluation, informed judgment, and real-world testing.”
