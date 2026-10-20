<p align="center">
  <img src="images/Banner.png" alt="Banner: Tejpal Singh Sandhu, Full Stack &amp; AI Developer" width="100%" />
</p>

<br>

<h1 align="center">
Hi, I'm <b>Tejpal Singh Sandhu</b> 👋
</h1>

<h3 align="center">
Full Stack & AI Developer
</h3>

<p align="center">
I build full-stack web apps and LLM-powered tools, with a focus on clean backends and AI features I can measure.
</p>

<p align="center">
ECE @ TIET, Class of 2027 • Backend Enthusiast • Problem Solver
</p>

<br>

<p align="center">

<a href="https://github.com/TejpalSandhu">
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
</a>

<a href="https://linkedin.com/in/tejpalsandhu007">
<img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin" alt="LinkedIn" />
</a>

<a href="mailto:tejpal.s.sandhu007@gmail.com">
<img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail" alt="Email" />
</a>

</p>

---

# 👨🏻‍💻 About

I'm an **Electronics & Communication Engineering undergraduate** at **Thapar Institute of Engineering & Technology**, graduating in **June 2027**.

I build web products end to end and add AI features where they help: an AI website builder with billing and version history, and a RAG support assistant whose retrieval I measured on a labelled test set before tuning it.

- 🎓 B.E. Electronics & Communication Engineering @ TIET (2023 – 2027)
- 💻 Full stack with React, TypeScript, Node.js, Express, PostgreSQL and MongoDB
- 🤖 AI engineering: RAG pipelines, vector search, LLM evaluation and tracing
- ⚙️ C++ and graph algorithms, applied to circuit netlists
- 📚 Practising DSA and system design (HLD & LLD)

---

# 🚀 Highlighted Projects

<p align="center">
Projects that best represent my work across full-stack development, AI and systems programming.
</p>

<br>

<table>
<tr>
<td width="50%" valign="top">

<a href="https://github.com/TejpalSandhu/forgesite-ai">
<img src="images/forgesite.png" alt="ForgeSite AI home page with a prompt box for describing a website" width="100%" />
</a>

### 🤖 ForgeSite AI

AI website builder: describe a site in one prompt, get a responsive page, then refine it by chatting with the AI or clicking elements to edit them.

- Two-stage LLM pipeline (prompt enhancement → HTML generation) runs in the background; credits are refunded automatically if generation fails
- Version history with rollback, iframe visual editor, phone / tablet / desktop preview, community publishing and HTML download
- 8-model PostgreSQL schema with Prisma, 13 REST endpoints, Better Auth sessions and Stripe webhooks for 3 credit plans

**Tech Stack**

`React` • `TypeScript` • `Tailwind CSS` • `shadcn/ui` • `Node.js` • `Express` • `PostgreSQL` • `Prisma` • `Better Auth` • `OpenRouter` • `Stripe`

<p>
<a href="https://github.com/TejpalSandhu/forgesite-ai">
<img src="https://img.shields.io/badge/Repository-181717?style=for-the-badge&logo=github" alt="ForgeSite AI repository" />
</a>
<a href="https://forgesite-ai-sepia.vercel.app/">
<img src="https://img.shields.io/badge/Live_Demo-0A66C2?style=for-the-badge&logo=vercel&logoColor=white" alt="ForgeSite AI live demo" />
</a>
</p>

</td>

<td width="50%" valign="top">

<a href="https://github.com/TejpalSandhu/support-rag-assistant">
<img src="images/rag-assistant.png" alt="Support RAG Assistant pipeline and results: 100% hit@5, MRR 0.91, 8 of 8 out-of-scope questions refused, 0 hallucinated answers" width="100%" />
</a>

### 🧠 Support RAG Assistant

Customer-support assistant that answers questions from 113 pages of 3D-printer manuals with page citations, and says so when the manuals don't cover a question.

- Gemini embeddings in a persistent ChromaDB index; content-hashed chunk IDs mean re-runs only embed new or changed text
- Compared 5 chunk settings on 28 labelled questions (100% hit@5, MRR 0.91) and cut the prompt context from 12 to 5 chunks
- Similarity threshold + grounded prompt refused 8 of 8 out-of-scope questions with 0 hallucinated answers; every request is traced in Langfuse

**Tech Stack**

`Python` • `Gemini API` • `ChromaDB` • `Langfuse` • `pypdf`

<p>
<a href="https://github.com/TejpalSandhu/support-rag-assistant">
<img src="https://img.shields.io/badge/Repository-181717?style=for-the-badge&logo=github" alt="Support RAG Assistant repository" />
</a>
</p>

</td>
</tr>

<tr>
<td width="50%" valign="top">

<a href="https://github.com/TejpalSandhu/CodeSphere">
<img src="images/codesphere.png" alt="CodeSphere landing page for collaborative coding interviews" width="100%" />
</a>

### 🚀 CodeSphere

Platform for 1-on-1 technical interviews: video call, chat, a Monaco code editor and code execution in one room.

- Runs JavaScript, Python, Java and C++ through the Judge0 API and checks the output against each problem's expected result
- 7 REST endpoints behind Clerk auth; Clerk JWTs are sent as bearer tokens so the Vercel frontend and Render backend work across domains
- 2 Inngest event-driven functions keep users in sync across Clerk, MongoDB and Stream

**Tech Stack**

`React` • `Tailwind CSS` • `daisyUI` • `TanStack Query` • `Node.js` • `Express` • `MongoDB` • `Clerk` • `Stream SDK` • `Judge0` • `Inngest`

<p>
<a href="https://github.com/TejpalSandhu/CodeSphere">
<img src="https://img.shields.io/badge/Repository-181717?style=for-the-badge&logo=github" alt="CodeSphere repository" />
</a>
<a href="https://code-sphere-kappa-seven.vercel.app/">
<img src="https://img.shields.io/badge/Live_Demo-0A66C2?style=for-the-badge&logo=vercel&logoColor=white" alt="CodeSphere live demo" />
</a>
</p>

</td>

<td width="50%" valign="top">

<a href="https://github.com/TejpalSandhu/netlist-connectivity-checker">
<img src="images/netlist-checker.png" alt="Terminal output of netcheck reporting two floating nodes in a sample netlist" width="100%" />
</a>

### ⚡ Netlist Connectivity Checker

C++17 command-line tool that checks SPICE-style circuit netlists for connectivity problems and input errors.

- Models the circuit as a graph (nodes as vertices, components as edges) and finds floating nodes with a breadth-first search from ground
- Reports malformed lines, unsupported components, invalid values (SPICE suffixes like `10k`, `1meg`) and duplicate names, each with its line number
- Parser, graph and report are separate modules covered by 30 unit tests; exit codes make it usable in scripts

**Tech Stack**

`C++17` • `g++` • `Graph algorithms`

<p>
<a href="https://github.com/TejpalSandhu/netlist-connectivity-checker">
<img src="https://img.shields.io/badge/Repository-181717?style=for-the-badge&logo=github" alt="Netlist Connectivity Checker repository" />
</a>
</p>

</td>
</tr>
</table>

### 🧩 More Projects

- **[CartPole AI](https://github.com/TejpalSandhu/CartPole_AI)**: Deep Q-Network agent that learns to balance a pole, with a FastAPI backend and a Streamlit dashboard for live training, playback, analytics and dual-agent and hurdle modes. `Python` • `PyTorch` • `Gymnasium` • `FastAPI` • `Streamlit`
- **[Dynamic CV Builder](https://github.com/TejpalSandhu/cv-application)** ([live demo](https://tejpalsandhu.github.io/cv-application/)): resume builder with live preview, customization and PDF export. `React` • `JavaScript` • `CSS`

---

# ⚙️ Technologies

<div align="center">
<table>
<tr>
<td valign="top" width="50%">

### 💻 Languages
<p>
<img src="https://skillicons.dev/icons?i=cpp,c,py,js,ts" alt="C++, C, Python, JavaScript, TypeScript" />
</p>

**Also:** SQL

</td>
<td valign="top" width="50%">

### 🎨 Frontend
<p>
<img src="https://skillicons.dev/icons?i=react,html,css,tailwind,vite" alt="React, HTML, CSS, Tailwind CSS, Vite" />
</p>

**Also:** TanStack Query • shadcn/ui • daisyUI • Monaco Editor

</td>
</tr>

<tr>
<td valign="top">

### ⚙️ Backend
<p>
<img src="https://skillicons.dev/icons?i=nodejs,express,fastapi" alt="Node.js, Express, FastAPI" />
</p>

- REST API design
- Auth: Clerk, Better Auth, JWT
- Payments: Stripe Checkout & webhooks
- Real-time: WebSockets, Stream video & chat SDK
- Background jobs: Inngest

</td>
<td valign="top">

### 🗄️ Databases & ORM / ODM
<p>
<img src="https://skillicons.dev/icons?i=postgres,mongodb,mysql,prisma" alt="PostgreSQL, MongoDB, MySQL, Prisma" />
</p>

- PostgreSQL • MongoDB • MySQL
- ChromaDB (vector database)
- Prisma • Mongoose • Sequelize

</td>
</tr>

<tr>
<td valign="top">

### 🤖 AI / ML
<p>
<img src="https://skillicons.dev/icons?i=pytorch" alt="PyTorch" />
</p>

- RAG, embeddings & vector search
- LLM evaluation (hit@k, MRR) & guardrails
- LLM tracing with Langfuse
- Gemini API • OpenRouter
- Deep Q-Learning (PyTorch, Gymnasium)

</td>
<td valign="top">

### 🛠️ Tools & Platforms
<p>
<img src="https://skillicons.dev/icons?i=git,github,vscode,postman,vercel" alt="Git, GitHub, VS Code, Postman, Vercel" />
</p>

- Claude Code
- Render

</td>
</tr>

<tr>
<td valign="top">

### 🧠 CS Fundamentals
- Data Structures & Algorithms
- Object-Oriented Programming
- DBMS • Operating Systems • Computer Networks
- System Design (HLD & LLD)

</td>
<td valign="top">

### 📚 Currently Exploring
- Docker
- AWS
- CI/CD
- Hybrid search & re-ranking for RAG

</td>
</tr>
</table>
</div>

---

# 📈 GitHub Analytics

<p align="center">

<img height="170" src="https://github-readme-stats-five-pi-3ajjvy7k5v.vercel.app/api?username=TejpalSandhu&show_icons=true&theme=github_dark&hide_border=true&rank_icon=github" alt="GitHub stats" />

<img height="170" src="https://github-readme-stats-five-pi-3ajjvy7k5v.vercel.app/api/top-langs/?username=TejpalSandhu&layout=compact&theme=github_dark&hide_border=true" alt="Most used languages" />

</p>

<p align="center">

<img src="https://streak-stats.demolab.com?user=TejpalSandhu&theme=github-dark&hide_border=true" alt="GitHub contribution streak" />

</p>

---

# 🤝 Let's Connect

<p align="center">
<a href="https://github.com/TejpalSandhu"><img src="https://skillicons.dev/icons?i=github" height="45" alt="GitHub" /></a>&nbsp;&nbsp;&nbsp;<a href="https://linkedin.com/in/tejpalsandhu007"><img src="https://skillicons.dev/icons?i=linkedin" height="45" alt="LinkedIn" /></a>&nbsp;&nbsp;&nbsp;<a href="mailto:tejpal.s.sandhu007@gmail.com"><img src="https://skillicons.dev/icons?i=gmail" height="45" alt="Email" /></a>
</p>

<p align="center">
<i>Thanks for visiting my profile! Feel free to explore my repositories or connect with me.</i>
</p>
