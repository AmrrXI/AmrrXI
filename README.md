<div align="center">

<img src="https://capsule-render.vercel.app/api?type=soft&height=170&color=0:0B1020,55:7C5CFF,100:22D3EE&text=Amr%20Tamer%20Hussein&fontSize=44&fontColor=FFFFFF&fontAlignY=40&desc=Agentic%20AI%20Developer%20%C2%B7%20LLMs%20%C2%B7%20Machine%20Learning&descSize=17&descAlignY=64&animation=fadeIn" width="100%" alt="Amr Tamer Hussein — Agentic AI Developer" />

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=19&duration=3200&pause=900&color=7C5CFF&center=true&vCenter=true&width=780&height=55&lines=I+build+AI+agents+that+plan%2C+pick+tools%2C+and+finish+the+job;LangGraph+%C2%B7+RAG+%C2%B7+Tool+calling+%C2%B7+Whisper+%C2%B7+Streamlit;From+raw+data+to+a+deployed+app+%E2%80%94+end+to+end" alt="What I do" />

<br>

<a href="https://www.linkedin.com/in/amr-tamer-9786a824">
  <img src="https://img.shields.io/badge/LinkedIn-7C5CFF?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>
<a href="mailto:amrrtamerr@hotmail.com">
  <img src="https://img.shields.io/badge/Email%20me-F59E0B?style=for-the-badge&logo=microsoftoutlook&logoColor=white" alt="Email" />
</a>
<a href="https://github.com/AmrrXI">
  <img src="https://img.shields.io/badge/GitHub-0B1020?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
</a>
<img src="https://img.shields.io/badge/New%20Cairo,%20Egypt-22D3EE?style=for-the-badge&logo=googlemaps&logoColor=white" alt="Location" />

<img src="https://komarev.com/ghpvc/?username=AmrrXI&label=Profile%20views&color=7C5CFF&style=flat-square" alt="Profile views" />

</div>

---

## About

AI graduate from the **Egyptian Russian University**, now building **agentic systems** — LLMs that read a request, choose a tool, run it, and come back with something finished. Before the agents, the same instinct in classic ML: clean the data, train the model, then actually ship it as an app someone can open.

- 🤖 **Agents & LLMs** — LangChain, LangGraph, tool calling, output parsing, RAG
- 🧠 **Deep learning** — CNNs and RNNs in TensorFlow, Keras, PyTorch
- 📊 **Data** — cleaning, analysis, visualization, and modelling in Python
- 🚀 **Shipping** — Streamlit apps, API integrations, error handling and retries
- 💬 Ask me about **agent design, RAG pipelines, or getting an LLM to behave**

<sub>🎯 Open to **AI / ML** and **Data Science** roles — remote or Cairo-based.</sub>

---

## How I build

Every project below is a version of this loop. Here it is as it runs in my meeting assistant:

```mermaid
flowchart LR
    IN([Meeting input<br/>text · pdf · audio]):::io
    W[Whisper<br/>speech-to-text]:::tool
    S[Summarizer<br/>agent]:::agent
    T[Task extractor<br/>agent]:::agent
    O[Owner assigner<br/>agent]:::agent
    D[Deadline detector<br/>agent]:::agent
    OUT([Summary + owned<br/>action items + PDF]):::io

    IN --> W --> S --> T --> O --> D --> OUT
    D -.->|missing context| S

    classDef agent fill:#7C5CFF,stroke:#22D3EE,stroke-width:1px,color:#FFFFFF
    classDef tool fill:#0B1020,stroke:#22D3EE,stroke-width:1px,color:#22D3EE
    classDef io fill:#F59E0B,stroke:#F59E0B,color:#0B1020
```

<sub>Four agents, one shared state, and a loop back when something is missing — not a single prompt pretending to be a product.</sub>

---

## Projects

<table>
<tr>
<td width="50%" valign="top">

### 📝 [Multi-Agent Meeting Assistant](https://github.com/AmrrXI/multi-agent-productivity-assistant)

Four LangGraph agents turn a raw meeting — text, PDF, or audio — into a summary, action items **assigned to the right owner**, and detected deadlines. Whisper handles the audio, and the whole thing exports as a PDF report.

<sub>**The hard part:** keeping four agents on one shared state without them overwriting each other.</sub>

<img src="https://img.shields.io/badge/LangGraph-7C5CFF?style=flat-square&logo=langgraph&logoColor=white" /> <img src="https://img.shields.io/badge/Whisper-7C5CFF?style=flat-square&logo=openai&logoColor=white" /> <img src="https://img.shields.io/badge/Groq-7C5CFF?style=flat-square" /> <img src="https://img.shields.io/badge/Streamlit-7C5CFF?style=flat-square&logo=streamlit&logoColor=white" />

</td>
<td width="50%" valign="top">

### 🤖 [LLM-Agent-Toolkit](https://github.com/AmrrXI/LLM-Agent-Toolkit)

An agent that reads a request, selects the right tool, and executes it — scheduling, location lookups, analytics. A rule-based fallback catches the cases the model isn't sure about, so it never dead-ends on the user.

<sub>**The hard part:** validating tool arguments with Pydantic before anything runs.</sub>

<img src="https://img.shields.io/badge/Qwen-7C5CFF?style=flat-square" /> <img src="https://img.shields.io/badge/Transformers-7C5CFF?style=flat-square&logo=huggingface&logoColor=white" /> <img src="https://img.shields.io/badge/Pydantic-7C5CFF?style=flat-square&logo=pydantic&logoColor=white" /> <img src="https://img.shields.io/badge/Groq-7C5CFF?style=flat-square" />

</td>
</tr>
<tr>
<td width="50%" valign="top">

### ⚽ [Football Knowledge Assistant](https://github.com/AmrrXI/Football-Knowledge-Assistant)

A RAG chatbot over a custom football knowledge base, with conversational memory — so "and who did he play for before that?" still knows who *he* is.

<sub>**The hard part:** chunking the knowledge base so retrieval returns the answer, not just the topic.</sub>

<img src="https://img.shields.io/badge/LangChain-22D3EE?style=flat-square&logo=langchain&logoColor=white" /> <img src="https://img.shields.io/badge/FAISS-22D3EE?style=flat-square" /> <img src="https://img.shields.io/badge/Groq-22D3EE?style=flat-square" />

</td>
<td width="50%" valign="top">

### ✉️ [AI Email Assistant](https://github.com/AmrrXI?tab=repositories)

An LLM pipeline that drafts professional replies and then handles the boring half — formatting, sending, saving, logging — through API-style functions with retries and proper error handling.

<sub>**The hard part:** failing gracefully. An agent that half-sends an email is worse than one that stops.</sub>

<img src="https://img.shields.io/badge/LLM%20Pipeline-22D3EE?style=flat-square" /> <img src="https://img.shields.io/badge/API%20Automation-22D3EE?style=flat-square" /> <img src="https://img.shields.io/badge/Python-22D3EE?style=flat-square&logo=python&logoColor=white" />

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📄 [HireHub — Applicant Tracking System](https://github.com/AmrrXI/ATS-using-Streamlit)

<sub>🎓 **Graduation project · Grade A · Team leader**</sub>

Parses CVs with NLP, scores them against a job description, and ranks the shortlist — so a hiring team reads five CVs instead of five hundred.

<sub>**The hard part:** ranking that survives messy, inconsistent CV formatting.</sub>

<img src="https://img.shields.io/badge/Python-F59E0B?style=flat-square&logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/Streamlit-F59E0B?style=flat-square&logo=streamlit&logoColor=white" /> <img src="https://img.shields.io/badge/NLP-F59E0B?style=flat-square" />

</td>
<td width="50%" valign="top">

### 💬 [Sentiment Analysis](https://github.com/AmrrXI/Sentiment-Analysis)

Sentiment and emotion classification over text, with the full preprocessing pipeline — tokenization, cleaning, normalization — and results visualized rather than printed.

<sub>**The hard part:** preprocessing that keeps the signal negation and sarcasm carry.</sub>

<img src="https://img.shields.io/badge/NLTK-F59E0B?style=flat-square" /> <img src="https://img.shields.io/badge/Matplotlib-F59E0B?style=flat-square" /> <img src="https://img.shields.io/badge/scikit--learn-F59E0B?style=flat-square&logo=scikitlearn&logoColor=white" />

</td>
</tr>
</table>

<sub>🔐 Also: [**Image Steganography**](https://github.com/AmrrXI/Image-Steganography) — hide and recover messages inside images, wrapped in a small Tkinter desktop app.</sub>

---

## Toolbox

<div align="center">
<img src="https://skillicons.dev/icons?i=py,java,postgres,tensorflow,pytorch,sklearn,anaconda,git,github,html,css&theme=dark&perline=11" alt="Core stack" />
</div>

<table>
<tr>
<td><b>Agentic AI & LLMs</b></td>
<td>
<img src="https://img.shields.io/badge/LangChain-7C5CFF?style=flat-square&logo=langchain&logoColor=white" />
<img src="https://img.shields.io/badge/LangGraph-7C5CFF?style=flat-square&logo=langgraph&logoColor=white" />
<img src="https://img.shields.io/badge/Hugging%20Face-7C5CFF?style=flat-square&logo=huggingface&logoColor=white" />
<img src="https://img.shields.io/badge/RAG-7C5CFF?style=flat-square" />
<img src="https://img.shields.io/badge/Tool%20Calling-7C5CFF?style=flat-square" />
<img src="https://img.shields.io/badge/Prompt%20Engineering-7C5CFF?style=flat-square" />
<img src="https://img.shields.io/badge/Output%20Parsing-7C5CFF?style=flat-square" />
<img src="https://img.shields.io/badge/FAISS-7C5CFF?style=flat-square" />
<img src="https://img.shields.io/badge/Groq-7C5CFF?style=flat-square" />
<img src="https://img.shields.io/badge/Gemini-7C5CFF?style=flat-square&logo=googlegemini&logoColor=white" />
</td>
</tr>
<tr>
<td><b>ML & Deep Learning</b></td>
<td>
<img src="https://img.shields.io/badge/PyTorch-22D3EE?style=flat-square&logo=pytorch&logoColor=white" />
<img src="https://img.shields.io/badge/TensorFlow-22D3EE?style=flat-square&logo=tensorflow&logoColor=white" />
<img src="https://img.shields.io/badge/Keras-22D3EE?style=flat-square&logo=keras&logoColor=white" />
<img src="https://img.shields.io/badge/scikit--learn-22D3EE?style=flat-square&logo=scikitlearn&logoColor=white" />
<img src="https://img.shields.io/badge/CNNs-22D3EE?style=flat-square" />
<img src="https://img.shields.io/badge/RNNs-22D3EE?style=flat-square" />
<img src="https://img.shields.io/badge/NLTK-22D3EE?style=flat-square" />
</td>
</tr>
<tr>
<td><b>Data & Analysis</b></td>
<td>
<img src="https://img.shields.io/badge/Pandas-F59E0B?style=flat-square&logo=pandas&logoColor=white" />
<img src="https://img.shields.io/badge/NumPy-F59E0B?style=flat-square&logo=numpy&logoColor=white" />
<img src="https://img.shields.io/badge/Matplotlib-F59E0B?style=flat-square" />
<img src="https://img.shields.io/badge/Seaborn-F59E0B?style=flat-square" />
<img src="https://img.shields.io/badge/SQL-F59E0B?style=flat-square&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/Jupyter-F59E0B?style=flat-square&logo=jupyter&logoColor=white" />
</td>
</tr>
<tr>
<td><b>Ship & Collaborate</b></td>
<td>
<img src="https://img.shields.io/badge/Streamlit-64748B?style=flat-square&logo=streamlit&logoColor=white" />
<img src="https://img.shields.io/badge/HTML5-64748B?style=flat-square&logo=html5&logoColor=white" />
<img src="https://img.shields.io/badge/CSS3-64748B?style=flat-square&logo=css3&logoColor=white" />
<img src="https://img.shields.io/badge/Git-64748B?style=flat-square&logo=git&logoColor=white" />
<img src="https://img.shields.io/badge/GitHub-64748B?style=flat-square&logo=github&logoColor=white" />
<img src="https://img.shields.io/badge/Jira-64748B?style=flat-square&logo=jira&logoColor=white" />
<img src="https://img.shields.io/badge/Agile%20%2F%20Scrum-64748B?style=flat-square" />
</td>
</tr>
</table>

---

## Training & credentials

Most recent first — the newer entries are where the agent work comes from.

| | Programme | Where | Focus |
|:--|:--|:--|:--|
| **Aug 2026** | AI & Technology | iCareer | AI-assisted workflows, Claude Code, task automation, Agile/Scrum, Jira, Git |
| **Jul 2026** | AI Agent Development | Digital Hub × Orange Digital Center | LLMs, LangChain, prompt engineering, agents, tool calling, API integration |
| **Sep 2024** | AI Practitioner Certificate | IBM | Hands-on ML, NLP and deep learning via Watson Studio |
| **Mar 2024** | ML Methods & Tools | IBM | Key algorithms applied to real-world datasets |
| **Mar 2024** | Fundamentals of AI | IBM | Core AI concepts and principles |
| **Sep 2023** | Artificial Intelligence | ITI × Arab Academy | AI basics, ML, DL, data science, Python |

🎓 **BSc Artificial Intelligence** — Egyptian Russian University, 2020–2024
🗣️ Arabic <sub>native</sub> · English <sub>upper-intermediate</sub> · Russian <sub>beginner</sub>

---

## The numbers

<div align="center">

<img height="165" src="https://github-stats-extended.vercel.app/api?username=AmrrXI&show_icons=true&hide_border=true&include_all_commits=true&count_private=true&rank_icon=github&bg_color=00000000&title_color=7C5CFF&text_color=94A3B8&icon_color=22D3EE" alt="GitHub stats" />
<img height="165" src="https://github-stats-extended.vercel.app/api/top-langs/?username=AmrrXI&layout=compact&langs_count=8&hide_border=true&bg_color=00000000&title_color=7C5CFF&text_color=94A3B8" alt="Top languages" />

<img height="165" src="https://streak-stats.demolab.com?user=AmrrXI&hide_border=true&background=00000000&stroke=7C5CFF&ring=22D3EE&fire=F59E0B&currStreakNum=7C5CFF&currStreakLabel=22D3EE&sideNums=94A3B8&sideLabels=94A3B8&dates=64748B" alt="Streak" />

<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=AmrrXI&bg_color=00000000&color=7C5CFF&line=22D3EE&point=F59E0B&area=true&area_color=7C5CFF&hide_border=true&custom_title=Commit%20activity" alt="Activity graph" />

<img src="https://github-profile-trophy.vercel.app/?username=AmrrXI&theme=algolia&no-frame=true&no-bg=true&margin-w=6&row=1&column=6" alt="Trophies" />

</div>

---

## Watch the snake eat my commits

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/AmrrXI/AmrrXI/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/AmrrXI/AmrrXI/output/github-snake.svg" />
  <img alt="Contribution grid, eaten by a snake" src="https://raw.githubusercontent.com/AmrrXI/AmrrXI/output/github-snake.svg" />
</picture>

</div>

---

<div align="center">

### Let's build something

I'm looking for **AI / ML** and **Data Science** work — and I'm happy to talk through an agent architecture with anyone who's stuck on one.

<a href="mailto:amrrtamerr@hotmail.com">
  <img src="https://img.shields.io/badge/Send%20me%20an%20email-F59E0B?style=for-the-badge&logo=microsoftoutlook&logoColor=white" alt="Email Amr" />
</a>
<a href="https://www.linkedin.com/in/amr-tamer-9786a824">
  <img src="https://img.shields.io/badge/Connect%20on%20LinkedIn-7C5CFF?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>

<sub>`amrrtamerr@hotmail.com` · +20 128 813 4755 · New Cairo, Egypt</sub>

<img src="https://capsule-render.vercel.app/api?type=waving&section=footer&height=110&color=0:22D3EE,45:7C5CFF,100:0B1020&reversal=true" width="100%" alt="" />

</div>
