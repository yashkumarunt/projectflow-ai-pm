# ProjectFlow – AI Project Management App (PartyRock + Bedrock)

👋 Hi, I’m **Yash Kumar Lal Das**.

**ProjectFlow** is an **AI-powered Project Management (PM) app** built with **Amazon PartyRock** (no-code UI) and **Amazon Bedrock** (LLM – Large Language Model).  
It converts a **backlog** into a **Kanban board** and a **capacity-aware sprint plan**, with both a **human-readable** and **JSON (JavaScript Object Notation)** output.

---

## ✨ Features
- **Kanban**: Auto-organize tasks into **To-Do / In-Progress / Blocked / Done**.
- **Sprint plan**: Capacity-aware schedule by **assignee** and **day**.
- **WIP (Work In Progress) limits**: Enforced to prevent overload.
- **Deadlines & priorities**: **H/M/L** ordering respected.
- **Dual output**: Human table + strict **JSON schema**.
- **Risks & next actions**: Clear, actionable summary.

---

## 🚀 Live Demo
> Add your public PartyRock link here once published  
`[https://partyrock.aws/u/YashKumar/E9mmmjXKi/ProjectFlow](url)`  

---

## 🧠 How It Works 
- You paste tasks and team info.
- The **AI (LLM – Large Language Model)** sorts and plans them.
- You get a **board (Kanban)** and a **schedule (sprint)**.
- We keep a **JSON version** so it’s easy to save or integrate later.

---

## 🧩 Example Input
See `/examples/sample_input.txt` (backlog + team + config)

---

## 📊 Example Outputs
- **Human view**: `/examples/sample_schedule.md`
- **JSON view**: `/examples/sample_output.json`

## 🧱 JSON Schema (strict)
```json
{
  "project": "ProjectFlow",
  "timezone": "America/Chicago",
  "columns": ["To-Do","In-Progress","Blocked","Done"],
  "wip_limits": {"In-Progress": 3},
  "sprint_window": {"start":"YYYY-MM-DD","end":"YYYY-MM-DD"},
  "team": [
    {"name":"<Name>","role":"<Role>","daily_capacity_hours":N}
  ],
  "tasks": [
    {"id":"T-001","title":"...","priority":"H|M|L","size":N,"due":"YYYY-MM-DD|null","assignee":"<Name|null>","status":"<column>","tags":[],"notes":""}
  ],
  "plan": [
    {"date":"YYYY-MM-DD","assignee":"<Name>","blocks":[{"start":"HH:MM","end":"HH:MM","task_id":"T-001","notes":""}]}
  ],
  "unscheduled": [],
  "risks": [],
  "next_actions": []
}
