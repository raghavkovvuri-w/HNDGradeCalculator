# HNC/HND Digital Technologies Grade Calculator

A modern, responsive, single page tool to calculate overall qualification grades for HNC and HND Digital Technologies pathways. It supports Software Development and Programming and Cyber Security, and applies the correct HNC versus HND grading rules.

Created by **Dr Raghav Kovvuri**, Course Leader Digital Technologies, University Centre Peterborough.  
Contact: **raghav.kovvuri@ieg.ac.uk**
- Livelink: [Link] https://raghavkovvuri-w.github.io/HNDGradeCalculator/grade-calculator.html

---

## Contents

- [Overview](#overview)
- [How grading works](#how-grading-works)
- [File structure](#file-structure)
- [How to use](#how-to-use)
- [Worked examples](#worked-examples)
- [Accessibility](#accessibility)
- [Roadmap](#roadmap)
- [Credits](#credits)
- [Licence](#licence)

---

## Overview

- Pathway aware: Software and Cyber Security have different unit maps.
- HNC versus HND logic: HNC uses Level 4 units. HND uses Level 5 units only for the overall grade.
- Award rules reminder: the results panel summarises credit rules and compensation.
- No frameworks required: pure HTML, CSS, and JavaScript in a single file.
- Branded layout: header area for logo and a footer attribution block.

---

## How grading works

**Unit credit value:** 15 credits each.

**Points per grade:**

| Grade | Points per credit | Points per 15 credit unit |
|------|--------------------|---------------------------|
| Pass | 4                  | 60                        |
| Merit| 6                  | 90                        |
| Distinction | 8          | 120                       |
| U (Compensated) | 0      | 0                         |

**Overall grade bands** (maximum 960 points):

- Pass: 420 to 599
- Merit: 600 to 839
- Distinction: 840 and above

**Award rules (summary):**

- HNC overall grade uses all Level 4 units.
- HND overall grade uses Level 5 units only.
- You need 120 credits at the relevant level and at least 105 credits at Pass or better.
- A maximum of one 15 credit unit can be compensated with U.

The calculator shows points and the resulting overall grade based on these rules.

---

## File structure
HNDGradeCalculator/
├── assest/ # Image assets
├── grade-calculator.html # Main app
└── README.md
## How to use

1. Select Pathway  
   - Software Development and Programming  
   - Cyber Security
2. Select Qualification  
   - HNC (Level 4 only)  
   - HND (Levels 4 and 5, overall grade based only on Level 5 points)
3. Enter grades for each listed unit.  
   - For HND, choose exactly two optional Level 5 units.
4. Click Calculate Overall Grade.
5. Review the total points, overall grade, and the award rules reminder.  
   For HND, a Level 4 status note is shown for context, while the overall grade uses Level 5 points only.

---

## Worked examples

### Example A: HNC (Level 4 only)

Suppose a student earns 3 Distinctions, 3 Merits, and 2 Passes across Level 4 units.

Calculation:
- Distinction: 3 × 120 = 360  
- Merit: 3 × 90 = 270  
- Pass: 2 × 60 = 120

**Total points:** 360 + 270 + 120 = 750  
**Overall band:** Merit (600 to 839)  
**Result:** HNC Merit

### Example B: HND (Level 5 grade only)

Suppose at Level 5 the student has 2 Distinctions, 4 Merits, 2 Passes, including exactly two optional units.

Calculation:
- Distinction: 2 × 120 = 240  
- Merit: 4 × 90 = 360  
- Pass: 2 × 60 = 120

**Total points:** 240 + 360 + 120 = 720  
**Overall band:** Merit (600 to 839)  
**Result:** HND Merit

### Example C: HND with one compensated unit (U)

Level 5 grades: 1 Distinction, 5 Merits, 1 Pass, 1 U.

- Distinction: 1 × 120 = 120  
- Merit: 5 × 90 = 450  
- Pass: 1 × 60 = 60  
- U: 1 × 0 = 0

**Total points:** 120 + 450 + 60 + 0 = 630  
**Overall band:** Merit  
Award still requires 120 credits at Level 5 with at least 105 credits at Pass or better, and only one compensated 15 credit unit.

---

## Accessibility

- High contrast colours and legible font sizes.
- Focus styles on form controls.
- Semantic headings and labels for selectors.

You can extend this with ARIA descriptions for the results section and an explicit focus order note if needed.

---

## Roadmap

- Optional CSV import for grades
- Export summary as PDF
- Basic analytics view of grade distributions
- More explicit validation messages and a sticky summary header

---

## Credits

Created by **Dr Raghav Kovvuri**, Course Leader Digital Technologies, University Centre Peterborough.  
Email: **raghav.kovvuri@ieg.ac.uk**

---

## Licence

This project is provided for educational use. You may adapt and reuse it with appropriate credit to the author and University Centre Peterborough.







