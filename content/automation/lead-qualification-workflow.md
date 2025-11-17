# Lead Qualification Workflow – Example

This is a simplified, fictitious workflow designed to show how I structure lead qualification logic in a marketing context.

---

## 🎯 Goal
Identify which incoming leads are “cold”, “warm”, or “ready to buy”, based on simple behavior and information provided.

---

## ⚡ Trigger
**Contact fills out a general lead form**

Fields captured:
• Name  
• Email  
• Company (optional)  
• Interest level (dropdown)  
• How they heard about the brand  

---

## 🛠️ Workflow Steps

### 1. **Assign Default Lead Status**
Immediately after form submission →  
Set property: **Lead Status = New**

---

### 2. **Check Interest Level**
If the field “Interest Level” is:
- **High** → Tag as *Warm Lead*
- **Medium** → Tag as *MQL Candidate*
- **Low** → Tag as *Cold Lead*

Action:
- Update property **Lead Category** accordingly

---

### 3. **Check Engagement Behavior (Optional)**
If lead opens the first email within 24 hours:
- Increase score by **+10**
Else:
- Increase score by **+2** (engagement still low)

This simulates simple scoring logic.

---

### 4. **Basic Lead Scoring Rules**
Score adjustments:
- +10 for high interest  
- +5 for medium interest  
- +2 for low interest  
- +10 for email open  
- +5 for clicking the CTA  
- +15 for visiting the pricing page  

Total score is updated under property:  
**Lead Score**

---

### 5. **Qualification Branch**
If **Lead Score ≥ 25**  
→ Mark as **MQL (Marketing Qualified Lead)**  
→ Notify the team or create a follow-up task

If **Lead Score < 25**  
→ Keep as **Nurture Lead**  
→ Add to nurture workflow  
→ No team task

---

### 6. **Optional: Route MQL to Sales**
If marked as MQL:
- Assign to team member  
- Create task: *"Review this lead – strong indicators"*  
- Send internal Slack/Email notification  

---

## 🧩 Logic Summary

• Captures full form info  
• Assigns default status  
• Categorizes lead by interest level  
• Applies simple lead scoring  
• Qualifies lead based on total score  
• Routes warm leads for follow-up  
• Sends cold leads to nurture  

---

## 📝 Notes

This workflow demonstrates:
• Basic lead qualification strategy  
• Clean scoring rules  
• CRM property updates  
• How to separate MQLs from cold leads  
• Professional workflow documentation  
