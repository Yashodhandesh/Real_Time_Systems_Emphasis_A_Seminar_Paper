# Real_Time_Systems_Emphasis_A_Seminar_Paper

# Handling Aperiodic Overloads

 # Overleaf link access : https://www.overleaf.com/read/yvbznrpprmxq#e913c4

 # 📘 Handling Aperiodic Overloads – Seminar Paper

**Course:** Real-Time Systems – Special Emphasis A  
**Institution:** Hamm-Lippstadt University of Applied Sciences, Germany  
**Author:** Yashodhan Vishvesh Deshpande  
**Email:** yashodhan-vishvesh.deshpande@stud.hshl.de  
**Repository:** [Real_Time_Systems_Emphasis_A_Seminar_Paper](https://github.com/Yashodhandesh/Real_Time_Systems_Emphasis_A_Seminar_Paper)

---

## 📝 Abstract

Modern real-time systems are increasingly subjected to **aperiodic task overloads**, which pose a significant risk to system reliability—particularly in **hard real-time environments**. This seminar paper presents a detailed study on **handling aperiodic overloads** through various scheduling strategies and algorithms.

Topics explored include:

- Periodic vs Aperiodic tasks  
- Overload types (Transient vs Permanent)  
- Cumulative value and competitive factor of algorithms  
- RED (Robust Earliest Deadline) algorithm  
- Dynamic Priority Exchange and Slack-Stealing algorithms  

---

## 📄 Table of Contents

1. [Introduction](#-introduction)
2. [Overload Types](#-overload-types)
3. [Key Concepts](#-key-concepts)
4. [RED Algorithm](#-red-robust-earliest-deadline-algorithm)
5. [Other Approaches](#-overview-of-other-algorithms)
6. [Conclusion](#-conclusion)
7. [References](#-references)

---

## 🔍 Introduction

The paper introduces the distinction between **periodic** and **aperiodic tasks** in real-time computing, and explains how **event-triggered scheduling** can cause unpredictable aperiodic overloads that may lead to **domino failures** in hard real-time systems.

---

## ⚠️ Overload Types

### 1. Transient Overload  
Short-term overloads where processor load `p(t) > 1` for a brief interval.

### 2. Permanent Overload  
Sustained overloads where average load exceeds capacity for a prolonged period.

---

## 📊 Key Concepts

- **Cumulative Value**: Prioritizes execution of more critical tasks during overloads.
- **Competitive Factor**: Measures the effectiveness of scheduling compared to an ideal (clairvoyant) scheduler.
- **Algorithm Classification**:
  - Best Effort
  - Acceptance Test Based
  - Robust Algorithms (e.g., RED)

---

## 🧠 RED – Robust Earliest Deadline Algorithm

RED extends the **Earliest Deadline First (EDF)** algorithm with:
- **Deadline tolerance (M)**
- **Residual laxity (L)**
- **Tolerance test (E)**  
- **Task rejection queues for missed deadlines**

RED enables **controlled degradation** and **resource reclaiming**, making it suitable for **soft real-time multimedia systems**.

A C implementation example is provided in the paper to illustrate how RED handles infeasible and tolerant tasks.

---

## 🔄 Overview of Other Algorithms

### ✅ Dynamic Priority Exchange  
- Prioritizes incoming aperiodic tasks  
- May delay periodic tasks  
- Simple but risky for hard RT systems

### ✅ Slack-Stealing  
- Fills gaps between periodic tasks with aperiodic jobs  
- Ensures deadline safety for periodic tasks  
- Less effective for long-duration aperiodic overloads

---

## 🧾 Conclusion

The paper outlines a complete framework for understanding, evaluating, and implementing scheduling algorithms to handle aperiodic overloads in real-time systems. RED, in particular, offers a practical compromise between system safety and flexibility.

---

## 📚 References

1. Buttazzo, G. – *Hard Real-Time Computing Systems*, Springer, 2011.  
2. Spuri, M., Buttazzo, G., Sensini, F. – *Robust Aperiodic Scheduling under Dynamic Priority Systems*  
3. Spuri, M., Buttazzo, G. – *Scheduling Aperiodic Tasks in Dynamic Priority Systems*, Real-Time Systems, 1996.  
4. Thuel, Lehoczky – *Slack Stealing in Fixed-Priority Systems*, RTSS, IEEE 1994.

---

## 📎 Repository Contents

| File | Description |
|------|-------------|
| `Real_time_systems_Final_seminar_paper.pdf` | Full seminar paper with references and diagrams |
| *(Optional: add code files or presentation slides here)* |

---

## 🔖 License

*(Specify here if this repository has a license, e.g. MIT, CC BY-NC-SA, or leave blank if none)*

---

## 🙋 Contact

Feel free to reach out for questions or collaborations:

**Yashodhan Vishvesh Deshpande**  
✉️ yashodhan-vishvesh.deshpande@stud.hshl.de  
📍 Hamm-Lippstadt University of Applied Sciences


