# Drafting Audit Plans

→ Just like architects design buildings, we (as lead implementers) need to plan out the audit process properly.

→ Drafting audit plans = laying out the full audit process on paper → then adjusting it to fit both the org’s and auditor’s timelines.



## How I'm approaching it:

- Start by listing the **common criteria** in a spreadsheet
- Then for each control → note what kind of **evidence** or **output** is expected
- Helps to visualize everything in one place


## Example that made it clearer for me:

→ If the org is being audited on **availability**, the evidence could be:

- List of **regions + availability zones** from the org’s cloud provider
- Uptime reports or failover configurations

So I basically need to map:  
**Control** ↔ **Expected Output** ↔ **Owner/Responsible Person**



## Why this step matters:

- Keeps me + team on track  
- Fewer surprises during the actual audit  
- Easy to communicate timelines + expectations  


## Spreadsheet Example

# Simple SOC 2 Common Criteria Mapping


| #  | Control Area               | What Is the Control?                                         | What Evidence Do You Need?                          | Who Is Responsible?   |
|----|----------------------------|--------------------------------------------------------------|-----------------------------------------------------|-----------------------|
| 1  | **Control Environment**     | Commitment to integrity and ethics                           | Code of conduct, training records                  | HR / Compliance       |
| 2  |                            | Board oversight of internal control                          | Meeting minutes, audit reviews                     | Board / Executive     |
| 3  |                            | Management assigns responsibilities                         | Organizational chart, job descriptions             | HR                    |
| 4  | **Risk Management**         | Risk assessment process                                      | Risk register, threat models                       | InfoSec / Risk Team   |
| 5  |                            | Identifies and assesses risks to objectives                  | Risk analysis documents, vulnerability scans       | Risk Team             |
| 6  | **Control Activities**      | Org implements controls over systems                         | Access control lists, firewall rules               | IT / InfoSec          |
| 7  |                            | Ongoing evaluation of controls                               | Logs, incident reports                             | InfoSec / SOC         |
| 8  | **Communication**           | Ensures internal and external communication of controls      | Internal memos, meeting notes                      | HR / Legal           |
| 9  | **Monitoring**              | Monitors the effectiveness of controls                       | Monitoring dashboards, alert logs                  | SOC / NOC             |
| 10 | **Change Management**       | Manages changes that affect controls                         | Change request logs, updated policies             | IT / DevOps           |

