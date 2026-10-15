# SynapseGrid OS: Autonomous Academic Scheduling & Conflict Resolution Platform

> **SYNAPSE: A 3-Hour Buildathon | Department of AIML & AIC-JIT (Jyothy Institute of Technology)**  
> **Challenge Track:** The Timetable Challenge – Designing for Academic Administrators  
> **Product Philosophy:** *Complex inside. Calm on the surface.*  
> **Live Interactive Demo:** [https://thunderous-sprinkles-7e9ae7.netlify.app/](https://thunderous-sprinkles-7e9ae7.netlify.app/)

---

## 📌 Submission Overview (Mandatory Items)

### 1. Team Name
**Team SynapticAI** *(or your designated college team name)*

### 2. Interactive Prototype Link
🌐 **Live Hosted URL:** [https://thunderous-sprinkles-7e9ae7.netlify.app/](https://thunderous-sprinkles-7e9ae7.netlify.app/)

### 3. Solution Summary (180 words)
Academic timetable generation is not merely an algorithmic constraint satisfaction problem; it is an administrative cognitive bottleneck where one slot decision collides with thirteen competing institutional forces. **SynapseGrid OS** transforms this high-stress process into a calm, proactive decision workstation designed specifically for Academic Administrators and Timetable Coordinators. 

Rather than forcing administrators through tedious trial-and-error loops, SynapseGrid delivers instant clash detection, live constraint validation, and explainable AI recommendations that tell the administrator not just *what* room to choose, but *why*—evaluating capacity headroom, equipment tags, walking distance, and accessibility compliance. 

Crucially, SynapseGrid introduces the **"Beyond the List" Emergency Proxy & Domino Solver**: when faculty report sudden morning sick leaves, the system instantly matches qualified departmental substitutes within AICTE workload limits without destabilizing the weekly master schedule. SynapseGrid bridges computational rigor with administrative trust.

---

## 🔐 Role-Based Access Control (RBAC) & Secret Keys

To prevent unauthorized student/faculty tampering, SynapseGrid implements enterprise role-based security:

| Role | Access Level | Secret Key | Capabilities |
|---|---|---|---|
| **Read-Only Viewer** | Public / Students | None | View timetable, filter clashes, search courses. Drag & drop is **locked**. |
| **Timetable Coordinator** | Department Staff | `COORD@2026` | **Drag & drop lectures into Open Free Slots**, swap classes, edit slot course/room/faculty. |
| **Academic Administrator** | Root Authority | `ADMIN@2026` | **Add/Remove classrooms** (room name, capacity, equipment), **add/manage faculty members** (department, domain, AICTE cap), master timetable publish. |

---

## ⚡ The 13 Forces Handled

| Force | Hard Rule / Soft Preference | SynapseGrid Implementation |
|---|---|---|
| **1. Classroom Capacity** | Hard Constraint | Verified $\ge$ batch size with 10% safety buffer |
| **2. Faculty Availability** | Hard Constraint | Zero double-booking across departments |
| **3. Laboratory Requirements** | Hard Constraint | Special hardware/GPU/lab technician profile tagging |
| **4. Semester Allocations** | Hard Constraint | Inter-semester core slot non-overlap |
| **5. Building Proximity** | Soft Preference | Adjacent class walking distance minimized (<180m) |
| **6. Accessibility** | Hard Constraint | Ground floor / elevator-serviced rooms enforced for mobility needs |
| **7. Classroom Equipment** | Soft Preference | Projector, smart-board, and audio system matching |
| **8. Internal Examinations** | Hard Constraint | Exam block freeze windows prevent scheduling clashes |
| **9. College Events** | Soft Preference | Auditorium and seminar hall blackout synchronization |
| **10. Maintenance Windows** | Hard Constraint | Periodic lab servicing and sanitization periods blocked |
| **11. Faculty Workload** | Hard Constraint | AICTE workload compliance (<16 teaching hours/week) |
| **12. Timetable Conflicts** | Hard Constraint | Instant visual flag with zero cognitive ambiguity |
| **13. Department Preferences** | Soft Preference | Departmental floor clustering and preferred lab hours |

---

## 🚀 Key Features

1. **Instant Clash Flagging (<5 sec spotting):** High-visibility red pulse cards with zero cognitive clutter.
2. **Explainable AI Recommendation Drawer (XAI):** Clear rationale for every suggested room relocation (capacity, projector tags, walking distance, accessibility).
3. **Faculty Message Portal with Strict 2-Chance Quota:**
   - Faculty can drop in-app messages to release slots.
   - Automatically re-plans the class and pushes live updates to all students & teachers.
   - Enforces a strict institutional limit: **maximum 2 class exchanges per faculty per week**.
4. **2-Option Publish & Distribution Pop-Up:**
   - Option A: ☑️ *Share Complete Timetable* with students and department displays.
   - Option B: ☑️ *Share Personalized Timetable to Every Faculty* (tailored schedule showing only their classes with free hours blanked).
5. **Dual Theme Engine:** Instant toggle between futuristic Dark Mode and official university Light Mode.
6. **"Beyond the List" Feature — Emergency Faculty Proxy Engine:** 1-Click qualified substitution engine for sudden faculty medical leaves.
7. **Administrator Infrastructure Console:** Dynamic addition of classrooms, capacities, equipment tags, and faculty rosters.
8. **Downstream Blast Radius & Ripple Effect Simulation:** Calculates downstream impact before executing any relocation.

---

## 🛠️ Tech Stack

* **Frontend:** Modern HTML5, Tailwind CSS, Lucide Icons, Chart.js, Canvas Confetti, Web Audio API synthesizer.
* **Architecture:** In-Memory Event-Driven Reactive State Engine with Role-Based Access Control.
* **Hosting:** Deployed live on Netlify via continuous static CDN.
