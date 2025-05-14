# Complementary User Entity Controls (CUECs)

## What I Learned

Complementary User Entity Controls (CUECs) are **controls that the customer (user entity)** is expected to implement in order to **support the effectiveness** of the service organization's controls. It's a **shared responsibility model**.

These controls **aren’t managed by the SaaS provider** — they fall on the **user organization's side**.

Think of it like this:
 The service provider handles their part of the control environment, but **some security and operational responsibilities must be handled by the customer**.


## Real-World Example (From the Course)

Let’s say there’s a company called **UI Automation Co.**  
They offer a SaaS product for **UI automation** that works on OS-level tasks (e.g., Windows/Mac), and provide a web platform where customers can:
- Monitor automation jobs
- Check job completion
- Use an emergency STOP button

Now, there’s another company called **Green Money Processing Inc.**, which uses UI Automation Co.’s platform to bridge legacy systems without APIs.

Here’s what went wrong:
- Green Money fired a developer who had **credentials to the UI Automation dashboard**.
- That person **logged in** and **deleted all the jobs** they had built — causing major disruption.

This **wasn't UI Automation Co.'s fault directly**, because they provided the access controls and UI. But Green Money failed to:
- Disable access for the former employee
- Enforce proper offboarding processes
- Use something like **SSO or 2FA**

So this is where a **CUEC** comes in:
UI Automation Co. should document in their **SOC 2 report** that *user entities are responsible for managing their own user access*.


## Why This Matters
- Auditors and customers need to **know where the responsibilities split**.
- If something goes wrong, it’s important to know whether the issue came from the **service provider** or the **user organization**.
- CUECs are typically listed in the SOC 2 report, under a section that says something like:
  > “The effectiveness of controls depends on certain controls implemented by user entities, including…”


## Key Takeaway
When reviewing or implementing SOC 2:
- **Identify CUECs in the service provider's report**
- **Map them to your own internal responsibilities**
- Make sure your **internal teams** are actually fulfilling those CUECs — especially access control, monitoring, data input validation, etc.

