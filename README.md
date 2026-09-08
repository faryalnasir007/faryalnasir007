from pathlib import Path

readme = """<div align="center">

# Faryal Nasir

### Full-Stack Engineer | .NET · React · Python · AI & Agentic Development

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Faryal%20Nasir-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/faryalnasir007/)

</div>

---

## 👩‍💻 About Me

Full-stack Engineer with **4+ years of experience**, having a strong foundation in software engineering and a growing focus on intelligent systems and AI. I combine analytical thinking with practical problem-solving to turn complex ideas into reliable, purposeful solutions.

Adaptable and research-oriented by nature, I enjoy exploring emerging technologies, understanding how systems behave, and continuously expanding the boundaries of what I can build and investigate.

---

## 💼 Work Experience

### Office of Superintendent of Public Instruction (OSPI)
**Full Stack Engineer** | Dec 2025 – Present  
*Olympia, WA, United States · Contract · Remote*  
[eVal](https://www.eval-wa.org)

The Office of Superintendent of Public Instruction is Washington State’s primary education agency, overseeing K–12 public education across the state and supporting nearly one million students through 295 school districts.

- Contribute to the redevelopment of **eVal**, a statewide educator evaluation system supporting structured teacher and principal evaluations, performance reviews, policy compliance, and accountability reporting.
- Develop full-stack modules for educator and administrator workflows, including evaluation cycles, evidence submission, scoring rubrics, performance tracking, and reporting.
- Build and integrate .NET-based REST APIs and backend functionality, implementing business logic and reliable data services.
- Develop responsive React-based dashboards and interfaces used by educators and administrators.
- Design and optimise SQL Server queries and database operations supporting large-scale educational, evaluation, and reporting data.
- Contribute to production support, debugging, testing, code reviews, and continuous platform enhancement.

**Tech:** `.NET` · `React` · `TypeScript` · `JavaScript` · `Python` · `HTML5` · `CSS3` · `Bootstrap` · `SQL Server` · `SQL`

---

### Namfus
**Full Stack Developer** | Jul 2025 – Nov 2025  
*Berlin, Germany · Contract · Remote*  
[Namfus](https://www.namfus.com)

Namfus is a student information and learning platform designed to enhance educational experiences through advanced management tools and AI-driven learning methods.

- Developed and enhanced full-stack functionality across core school administration and learning workflows.
- Built and maintained functionality for student records, attendance, courses, assessments and grading, timetabling, and related administrative workflows.
- Developed .NET backend functionality and REST APIs supporting interconnected platform modules.
- Built and enhanced responsive React-based interfaces and integrated front-end functionality with backend services.
- Worked with SQL Server to implement queries, data operations, and application functionality.
- Contributed to feature development, API integration, debugging, testing, and continuous improvement.

**Tech:** `.NET` · `React` · `TypeScript` · `JavaScript` · `HTML5` · `CSS3` · `Bootstrap` · `SQL Server` · `SQL`

---

### Contour Software
**Full Stack Developer** | Mar 2024 – Jun 2025  
*Lahore, Pakistan · Contract · Hybrid*  
[Contour Software](https://www.contour-software.com)

- Developed and enhanced full-stack business applications across front-end interfaces, backend services, application logic, APIs, and relational databases.
- Built .NET backend functionality covering business logic, data processing, integrations, and database-driven workflows.
- Developed responsive applications using React and Angular, creating reusable components and production-ready features.
- Contributed to AI-oriented communication and intelligent web platforms.
- Worked on education and professional learning functionality including courses, assessments, learner activities, progress, and credit tracking.
- Contributed across feature implementation, debugging, testing, maintenance, performance improvements, and production-system enhancement.

**Tech:** `.NET` · `React` · `TypeScript` · `JavaScript` · `HTML5` · `CSS3` · `Bootstrap` · `Tailwind CSS` · `APIs` · `SQL Server` · `SQL`

---

### The Dev Corporate
**Back-End Developer** | Jan 2023 – Feb 2024  
*Lahore, Pakistan · Contract · Onsite*  
[The Dev Corporate](https://www.thedevcorporate.com)

- Developed Python-based backend functionality for business and data-driven applications.
- Worked on data preprocessing, aggregation, trend identification, analysis, visualisation, and data-driven workflows.
- Developed backend functionality and REST APIs using .NET with relational database integrations.
- Contributed to AI-enabled application functionality and API integrations.
- Worked on payments, subscriptions, invoicing, customer management, authentication, and third-party integrations.
- Expanded into React-based front-end development and front-end/backend integration.

**Tech:** `Python` · `.NET` · `React` · `JavaScript` · `HTML5` · `CSS3` · `Bootstrap` · `REST APIs` · `SQL` · `SQL Server` · `MySQL` · `OpenAI API`

---

### XiCor
**Junior Web / UI Developer** | Jan 2022 – Dec 2022  
*Lahore, Pakistan · Contract · Hybrid · Part-Time*

- Developed and customised responsive web pages and user-interface components.
- Worked with WordPress websites including layouts, content integration, styling, and front-end customisation.
- Implemented responsive interfaces using HTML, SCSS, JavaScript, and Bootstrap.
- Translated UI designs and business requirements into functional web interfaces while completing undergraduate studies.

**Tech:** `WordPress` · `JavaScript` · `HTML5` · `CSS3` · `SCSS` · `Bootstrap`

---

## 🛠️ Technical Skills

**Back-End Development**  
`Python` · `.NET`

**Front-End Development**  
`React` · `HTML5` · `CSS3` · `SCSS` · `Bootstrap` · `Tailwind` · `TypeScript`

**Programming Languages**  
`Python` · `C#` · `SQL` · `JavaScript`

**AI & Agentic Development**  
`LangChain` · `LangGraph` · `CrewAI` · `OpenAI Agents SDK` · `OpenAI API`

**Workflow Automation**  
`n8n` · `Zapier AI`

**Development Environments**  
`Visual Studio` · `Visual Studio Code` · `SQL Server Management Studio`

---

## 🎓 Education

### BS Mechatronics & Control Engineering
**University of Engineering and Technology, Lahore** | 2018 – 2022  
*Lahore, Pakistan*

- **PEC Level-II Accredited (Washington Accord)**
- **EQF:** Level 6
- **Percentage:** 71.76%
- [University Website](https://www.uet.edu.pk)

---

## 🌐 Languages

**Urdu** · Mother tongue  
**Punjabi** · Mother tongue  
**English** · C2 Proficient

### Pearson Test of English (PTE Academic)

**Overall Score:** 90  
Listening: 90 · Reading: 87 · Speaking: 88 · Writing: 90  
**Validity:** 12 Dec 2025 – 12 Dec 2027  
**Score Report Code:** `44a9ab8PQF`

---

## 🤝 Soft Skills

`Adaptability` · `Emotional Intelligence` · `Time Management` · `Active Listening` · `Problem Solving` · `Collaboration` · `Effective Communication`

---

<div align="center">

### Connect with me on [LinkedIn](https://www.linkedin.com/in/faryalnasir007/)

</div>
"""

out = Path("/mnt/data/README_CLEAN.md")
out.write_text(readme, encoding="utf-8")

# Verify that removed private details do not exist anywhere in the file.
forbidden = [
    "fwahlah18@gmail.com",
    "306 4238780",
    "bit.ly/4zLCBaB",
    "35201-8053834-0",
    "18 Dec 2000",
    "Canal Bank Housing Scheme",
]
assert not any(x in readme for x in forbidden)

print("Created clean README_CLEAN.md")
print(f"{len(readme.splitlines())} lines")
