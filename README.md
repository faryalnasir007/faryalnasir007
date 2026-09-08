from pathlib import Path
import pypandoc

md = r"""# Faryal Nasir

**Full-Stack Engineer | .NET · React · Python · AI & Agentic Development**

Full-stack Engineer with 4+ years of experience, having a strong foundation in software engineering and a growing focus on intelligent systems and AI. I combine analytical thinking with practical problem-solving to turn complex ideas into reliable, purposeful solutions. Adaptable and research-oriented by nature, I enjoy exploring emerging technologies, understanding how systems behave, and continuously expanding the boundaries of what I can build and investigate.

## Contact

- **Location:** Lahore, Pakistan
- **Email:** fwahlah18@gmail.com
- **Phone:** (+92) 306 4238780
- **Portfolio:** https://bit.ly/4zLCBaB
- **LinkedIn:** Faryal Nasir
- **GitHub:** Faryal Nasir

## Work Experience

### Full Stack Engineer — Office of Superintendent of Public Instruction (OSPI)
**Olympia, WA, United States · Contract · Remote**  
**Dec 2025 – Present**  
**Department:** Education · **Website:** https://www.eval-wa.org

The Office of Superintendent of Public Instruction is Washington State’s primary education agency, overseeing K–12 public education across the state and supporting nearly one million students through 295 school districts.

- Contribute to the redevelopment of a statewide educator evaluation system, eVal, supporting structured teacher and principal evaluations, performance reviews, policy compliance, and accountability reporting.
- Develop full-stack modules for educator and administrator workflows, including evaluation cycles, evidence submission, scoring rubrics, performance tracking, and reporting.
- Build and integrate .NET-based REST APIs and backend functionality, implementing business logic and reliable data services for application workflows.
- Develop responsive React-based dashboards and interfaces used by educators and administrators across the evaluation process.
- Design and optimise SQL Server queries and database operations supporting large-scale educational, evaluation, and reporting data.
- Contribute to production support, debugging, testing, code reviews, and continuous enhancement of the statewide platform.

**Technologies:** .NET, React, TypeScript, JavaScript, Python, HTML5, CSS3, Bootstrap, SQL Server, SQL

### Full Stack Developer — Namfus
**Berlin, Germany · Contract · Remote**  
**Jul 2025 – Nov 2025**  
**Department:** Education · **Website:** https://www.namfus.com

Namfus is a student information and learning platform designed to enhance educational experiences through advanced management tools and AI-driven learning methods.

- Developed and enhanced full-stack functionality across core school administration and learning workflows, supporting day-to-day operations for educational institutions.
- Built and maintained functionality for student records, attendance, courses, assessments and grading, timetabling, and related administrative workflows.
- Developed .NET backend functionality and REST APIs, implementing business logic and data operations supporting interconnected platform modules.
- Built and enhanced React-based interfaces, creating responsive user workflows and integrating front-end functionality with backend services.
- Worked with SQL Server to implement queries, data operations, and application functionality across education-related modules.
- Contributed to feature development, API integration, debugging, testing, and continuous improvement of the production platform.

**Technologies:** .NET, React, TypeScript, JavaScript, HTML5, CSS3, Bootstrap, SQL Server, SQL

### Full Stack Developer — Contour Software
**Lahore, Pakistan · Contract · Hybrid**  
**Mar 2024 – Jun 2025**  
**Website:** https://www.contour-software.com

Contour Software is a software development and technology organisation delivering and supporting specialised business software products across multiple industries and international markets.

- Developed and enhanced full-stack business applications, working across front-end interfaces, backend services, application logic, APIs, and relational databases.
- Built .NET backend functionality, implementing business logic, data processing, integrations, and database-driven application workflows.
- Developed responsive and interactive applications using React and Angular, creating reusable components and translating functional and UI requirements into production-ready features.
- Contributed to AI-oriented communication and intelligent web platforms, focusing on modern front-end experiences, interactive functionality, and integration with application services.
- Worked on education and professional learning functionality, including courses, assessments, learner activities, progress and credit tracking, as one of several product domains supported during the role.
- Contributed across the software development lifecycle, including feature implementation, debugging, testing, code maintenance, performance improvements, and enhancement of established production systems.

**Technologies:** .NET, React, TypeScript, JavaScript, HTML5, CSS3, Bootstrap, Tailwind CSS, APIs, SQL Server, SQL

### Back-End Developer — The Dev Corporate
**Lahore, Pakistan · Contract · Onsite**  
**Jan 2023 – Feb 2024**  
**Website:** https://www.thedevcorporate.com

The Dev Corporate is a software development and technology services company delivering custom web, backend, data-driven, and business application solutions.

- Developed Python-based backend functionality for business and data-driven applications, working on application logic, data processing, and API-driven functionality.
- Worked on analytics and data-processing functionality, including data preprocessing, aggregation, trend identification, analysis, visualisation, and data-driven application workflows.
- Developed backend functionality and REST APIs using .NET, integrating relational databases to support application data and business processes.
- Contributed to AI-enabled application functionality and API integrations, incorporating intelligent and data-driven capabilities into web applications.
- Worked on business application modules covering payments, subscriptions, invoicing, customer management, authentication, and third-party integrations.
- Expanded into React-based front-end development, contributing to component-based interfaces and integration between front-end applications and backend services.

**Technologies:** Python, .NET, React, JavaScript, HTML5, CSS3, Bootstrap, REST APIs, SQL, SQL Server, MySQL, OpenAI API

### Junior Web / UI Developer — XiCor
**Lahore, Pakistan · Contract · Hybrid · Part-Time**  
**Jan 2022 – Dec 2022**

XiCor is a technology and digital solutions company providing web development and software services for business clients.

- Developed and customised responsive web pages and user-interface components based on project and design requirements.
- Worked with WordPress-based websites, including page layouts, content integration, styling, and front-end customisation.
- Implemented and refined responsive interfaces using HTML, SCSS, JavaScript, and Bootstrap.
- Gained practical experience translating UI designs and business requirements into functional web interfaces while completing undergraduate studies.

**Technologies:** WordPress, JavaScript, HTML5, CSS3, SCSS, Bootstrap

## Education

### BS Mechatronics & Control Engineering
**University of Engineering and Technology, Lahore**  
**2018 – 2022 · Lahore, Pakistan**

- **Website:** https://www.uet.edu.pk
- **EQF:** Level 6
- **Accreditation:** PEC Level-II Accredited (Washington Accord)
- **Percentage:** 71.76%

## Skills

### Back-End Development
`Python` · `.NET`

### Front-End Development
`React` · `HTML5` · `CSS3` · `SCSS` · `Bootstrap` · `Tailwind` · `TypeScript`

### Programming Languages
`Python` · `C#` · `SQL` · `JavaScript`

### AI & Agentic Development
`LangChain` · `LangGraph` · `CrewAI` · `OpenAI Agents SDK` · `OpenAI API`

### Workflow Automation
`n8n` · `Zapier AI`

### Development Environments
`Visual Studio` · `Visual Studio Code` · `SQL Server Management Studio`

### Soft Skills
`Adaptability` · `Emotional Intelligence` · `Time Management` · `Active Listening` · `Problem Solving` · `Collaboration` · `Effective Communication`

## Languages

- **Urdu:** Mother tongue
- **Punjabi:** Mother tongue
- **English:** C2 Proficient

### Pearson Test of English (PTE Academic)

- **Overall Score:** 90
- **Listening:** 90
- **Reading:** 87
- **Speaking:** 88
- **Writing:** 90
- **Validity:** 12 Dec 2025 – 12 Dec 2027
- **Score Report Code:** 44a9ab8PQF

## References

Available upon request.
"""

out = "/mnt/data/README.md"
pypandoc.convert_text(md, "md", format="md", outputfile=out, extra_args=["--standalone"])
print(f"Created {out}")

