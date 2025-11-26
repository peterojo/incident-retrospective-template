# 🛠️ Incident Retrospective Template

A simple, blameless, lightweight retrospective template for engineering teams.  
Use this to run fast, effective post-incident reviews and capture learnings that drive reliability improvements.

---

## 1. Summary

**Date:**  
**Duration:**  
**Severity / Impact Level:**  
**Affected Services:**  
**Reported By:**  
**Owner(s):**  

**Short summary (2–3 sentences):**  
High-level outline of what happened, what was impacted, and how it was resolved.

---

## 2. Timeline (UTC recommended)

| Time | Event |
|------|--------|
| 00:00 | Initial alert triggers |
| 00:02 | First responder acknowledges |
| 00:10 | Investigation begins |
| ... | ... |

Tips: keep events factual, chronological, and detailed enough to understand the sequence.

---

## 3. Impact

**Customer impact:**  
- (e.g., degraded API performance, failed checkouts, delayed notifications)

**Business impact:**  
- (e.g., 12% failure rate for 18 mins, 200 support tickets, revenue risk)

**Technical impact:**  
- (e.g., increased p95, DB CPU saturation)

---

## 4. Root Cause Analysis

Describe the underlying factors using one or more frameworks:
- **5 Whys**
- **Fishbone diagram (optional)**

**Example format:**
- Symptom: <what was observed>  
- Trigger: <what event caused it>  
- Root cause: <foundational issue>  

---

## 5. Contributing Factors

List non-root-cause elements that made the incident worse:
- Monitoring gaps  
- Missing rate limits  
- Unexpected traffic patterns  
- Unclear ownership  
- Knowledge silo  
- Slow or noisy alert

---

## 6. Detection & Response

**How was the issue detected?**  
**Were alerts effective?**  
**What slowed down resolution?**  
**Was communication adequate?**  

---

## 7. Resolution

**What fixed the issue?**  
Write the exact steps taken, e.g configs, rollbacks, restarts, scaling, feature flags, hotfixes.

---

## 8. Preventive Actions

Break these into three buckets:

### 🔧 Short-term fixes (this week)
- [ ] Improve alert thresholds  
- [ ] Add log for X failure path  
- [ ] Tighten dashboard panel  

### 🧱 Medium-term fixes (this quarter)
- [ ] Add retry strategy / circuit breaker  
- [ ] Infrastructure scaling improvements  
- [ ] Migrate dependency XYZ  

### 🧭 Long-term investments
- [ ] System redesign  
- [ ] Distributed tracing rollout  
- [ ] Operational maturity improvement  

Each action should include:
- Owner  
- Deadline  
- Priority  
- Status  

---

## 9. Lessons Learned

Bullet list of 3–10 insights the team wants to remember.

Examples:  
- “We investigated the wrong subsystem for 20 minutes due to ambiguous alerts.”  
- “Traffic pattern X now exceeds our assumed normal baseline.”  
- “Rollback procedures were unclear, needs docs.”

---

## 10. Appendix

- Logs, graphs, screenshots  
- Related incidents  
- Slack timeline  
- Links to dashboards  
- Code diffs (if relevant)

---

**Maintainers:** [your name or org]
