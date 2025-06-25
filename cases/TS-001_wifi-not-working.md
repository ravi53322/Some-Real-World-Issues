# TS-001 - WiFi Keeps Disconnecting on Windows 10

📅 Logged on: 25 June 2025  
🎯 Ticket Category: Networking  
🔧 Difficulty: Beginner

---

### 🧩 PROBLEM:

User reports WiFi disconnects every 5–10 minutes post-Windows update.

---

### 🧠 SUSPECTED CAUSES:

- Outdated or corrupted wireless driver  
- DHCP lease expired/not renewing  
- IP conflict or DNS cache fail

---

### 🛠️ TROUBLESHOOTING STEPS:

1. ✅ Checked Device Manager → Rollback driver  
2. ✅ Ran CMD: `ipconfig /release` & `ipconfig /renew`  
3. ✅ Flushed DNS: `ipconfig /flushdns`  
4. ✅ Checked router → no conflict  
5. ✅ Set static DNS (1.1.1.1 via adapter settings)

---

### ✅ FINAL RESOLUTION:

Connected user to stable network. Reset driver + DNS cleaned issue.  
Tested for 30 mins — STABLE.

---

### 📚 NOTE TO SELF:

🔹 Always backup network settings before changing  
🔹 Document adapter name + log 🧠  
🔹 Check Event Viewer if nothing visible  
