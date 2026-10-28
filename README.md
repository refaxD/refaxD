<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&pause=1200&color=00ADD8&center=true&vCenter=true&width=620&lines=Backend+developer+in+Go+and+Python;CI%2FCD%2C+Docker+and+Yandex+Cloud;RAG+and+LLM+pipelines+for+documents;Hackathon+team+lead+and+PM" alt="Typing intro" />

[![Telegram](https://img.shields.io/badge/Telegram-@refaxD-26A5E4?style=flat-square&logo=telegram&logoColor=white)](https://t.me/refaxD)
[![Email](https://img.shields.io/badge/Email-poddubnyanton8@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:poddubnyanton8@gmail.com)
![Currently](https://img.shields.io/badge/Now-Backend_at_IT__One-6E40C9?style=flat-square)
![Open to](https://img.shields.io/badge/Open_to-backend_roles-2EA44F?style=flat-square)
![Profile views](https://komarev.com/ghpvc/?username=refaxD&color=00ADD8&style=flat-square&label=views)

</div>

Backend developer in Go and Python, currently at IT_One. Student at Central University (B.S. in Mathematics and Computer Science, Software Engineering track, class of '29). I usually end up as team lead at hackathons, so I also handle requirements, priorities and the pitch.

---

### Experience

**IT_One**, Backend Developer · Jul 2026 to present
I write the APIs and business logic of an employee onboarding platform, cover the code with tests and take part in code review. I own the infrastructure and CI/CD on Jenkins and help with the React frontend.

**Nikta AI**, Backend Developer (Python) · Oct 2025 to Dec 2025 · [recommendation letter](https://drive.google.com/file/d/1Lw4P5dAIN0eI8TI2uRzVFqUL9MUDm96_/view?usp=sharing)
Ran the Dynamic Chunking project for RAG almost on my own, from requirements to deployment. I built an LLM pipeline that finds a document's logical boundaries and extracts metadata, cutting analysts' manual markup by about 80%, and wrapped it in a FastAPI service with Celery, Redis and Docker.

---

### Projects

#### [Veha](https://github.com/fadegor05/LCT-7) · Leaders of Digital Transformation 2026, finals
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![YOLO](https://img.shields.io/badge/YOLO-111F68?style=flat-square)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Yandex Cloud](https://img.shields.io/badge/Yandex_Cloud-5282FF?style=flat-square&logo=yandexcloud&logoColor=white)

Checks whether a construction site is on schedule from camera photos. YOLO finds machinery in each frame, and the backend groups photos by day and compares them with the work plan. On a real site in Berezniki it processed 904 frames from 4 cameras over 10 working days, and 19 of 20 stage statuses on the validation set matched manual labeling. The stand runs without a GPU at 0.73 s per frame. I was team lead, PM and backend developer in a team of 5.

<details>
<summary><b>What I did</b></summary>

- **Product.** Wrote up the Q&A session with the task owners and turned it into decisions, reviewed the MVP mockup against the spec and the API contract, and defined the demo dataset with a coverage matrix and a readiness criterion.
- **Research.** Measured observability on the current labeling (experiments E4, E5 and E11) and wrote five research branches: scene, activity, time, competitions, and a review of commercial construction monitoring products.
- **Infrastructure.** Set up the Yandex Cloud stand. GitHub Actions runs checks and builds images into Yandex Container Registry, and a systemd-timer agent pulls new versions and health-checks the stand by domain. During the open finals pitch the stand took traffic from every team that scanned our QR code.
- **Backend.** Walked through the stand as a user, filed 5 bug reports and fixed them: shooting date from the file name, statuses of stages with no data, readable API errors, a 500 on uploading photos with detections, and scheduled camera snapshots.
- **Frontend.** Built login and sign-up, a landing page with a live work schedule chart, a photo viewer with detector boxes, and fixes for the report assistant panel.

</details>

#### [NNKL Knowledge Graph](https://github.com/pxc1984/nnkl) · Nornickel case
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Gin](https://img.shields.io/badge/Gin-008ECF?style=flat-square&logo=gin&logoColor=white)
![LightRAG](https://img.shields.io/badge/LightRAG-5A4FCF?style=flat-square)
![Svelte](https://img.shields.io/badge/Svelte-FF3E00?style=flat-square&logo=svelte&logoColor=white)

Builds a knowledge graph from scientific papers and internal R&D reports and answers questions over it with links to the sources. I was team lead and a full-stack developer.

<details>
<summary><b>What I did</b></summary>

- **Question answering.** Wrote the Go `ask` endpoint on top of LightRAG. Answers cite the source files by name, type and date, with numbered references and no duplicate reference block.
- **Numeric constraints.** A separate enhancer parses limits like "sulfates ≤ 300 mg/L" or "melting point > 1000 °C" out of the question (less than, more than, between, with units) and adds them to the prompt. Both the endpoint and the enhancer are covered by tests.
- **Graph view.** Built the knowledge graph page on Svelte and Cytoscape and mapped LightRAG entity types to legend colors.
- **Heavy documents.** Wrote a standalone Python parser that extracts text from large PDFs through Yandex APIs.
- **API.** Shaped the OpenAPI contract and added upload diagnostics for large files.

</details>

#### [Code Leak Scanner](https://drive.google.com/file/d/1vU8NicIB7HcQRHltgZAJ1R8MIChIVSDs/view?usp=sharing) · Nuclear IT Hack, finals
Go (Fiber) workers stream-scan repositories for leaked secrets and talk to a FastAPI gateway over RabbitMQ. Moving pattern matching to AST parsing made scanning 1.5 times faster than the baseline.

---

### Tech stack

**Languages**
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)
![C](https://img.shields.io/badge/C-basic-A8B9CC?style=for-the-badge&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-basic-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)

**Backend**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Gin](https://img.shields.io/badge/Gin-008ECF?style=for-the-badge&logo=gin&logoColor=white)
![Fiber](https://img.shields.io/badge/Fiber-00ACD7?style=for-the-badge&logo=go&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=sqlalchemy&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white)

**Data and messaging**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)

**Infrastructure**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

**Practices**
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)
![mypy](https://img.shields.io/badge/mypy-2A6DB2?style=for-the-badge)
![Ruff](https://img.shields.io/badge/Ruff-D7FF64?style=for-the-badge&logo=ruff&logoColor=black)
![Code review](https://img.shields.io/badge/Code_review-24292F?style=for-the-badge&logo=github&logoColor=white)

**LLM and data**
![RAG](https://img.shields.io/badge/RAG_·_LightRAG-5A4FCF?style=for-the-badge)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)

**Frontend, enough to help the team**
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

---

### Analytics and business analysis, intern level

- **Data analysis.** SQL, Pandas and Matplotlib for exploring data and checking hypotheses. Four solved [analytics case studies](https://drive.google.com/drive/folders/17GCAiL4Y7YRD35BATDruhzj9E1nu0m_C?usp=sharing).
- **Business analysis.** Gathering requirements and setting priorities (at Nikta AI I owned both), turning Q&A sessions with task owners into decisions, and reviewing competitor products, as in Veha.

---

### Achievements

- [Winter CodeRun Challenge (Yandex)](https://drive.google.com/file/d/17ecS9IKzYDuUEIR_QcGMC1f1IEIlF_94/view?usp=sharing): overall winner, top 100, 59th place
- [Kod Sporta (T-Bank)](https://drive.google.com/file/d/1EScDgeyCg7Dzz7g2zVVGK3DFt7Cavgo-/view?usp=sharing): prize winner, top 10 of 70 teams, in person with no AI
- [Vladimir Potanin Scholarship](https://drive.google.com/file/d/1FFNaN2G7y5AALQUQxgq8c9tDcm2KQbQu/view?usp=sharing), 2026
- [CU School CTF](https://drive.google.com/file/d/1WBV-br6N7NDynUBMxZiX3rb-T8n7Flhc/view?usp=sharing): 2nd place
- [HSE CS x BRICS Hackathon](https://drive.google.com/file/d/1oFbwxLp0v97v06Arj_D00CcjUvD9KLBg/view?usp=sharing): winner

---

### GitHub stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=refaxD&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=refaxD&layout=compact&theme=tokyonight&hide_border=true" alt="Top languages" />

<img src="https://streak-stats.demolab.com?user=refaxD&theme=tokyonight&hide_border=true" alt="Streak" />

</div>

---

### Education

Central University, B.S. in Mathematics and Computer Science, Software Engineering track, class of '29.
Courses: Industrial Software Development, Go Development, Advanced Python Development, Algorithms and Data Structures, Computer Architecture and Operating Systems, Calculus, Linear Algebra, Discrete Mathematics.

<div align="center">

[![Resume](https://img.shields.io/badge/📄_Resume-FF0000?style=for-the-badge&logo=adobe-acrobat-reader&logoColor=white)](https://disk.yandex.ru/d/dzqUc1EW8bWezw)
[![Certificates](https://img.shields.io/badge/🏆_Certificates-4285F4?style=for-the-badge&logo=googledrive&logoColor=white)](https://drive.google.com/drive/folders/1_RWTvt1XrNhli87CtZL1qwQBlAg4aLL3?usp=sharing)

</div>
