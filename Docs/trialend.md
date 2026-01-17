
---

### **Step 1: Install Node.js (LTS)**

1. Go to **[https://nodejs.org](https://nodejs.org)**
2. Download **LTS version** (v18 or newer)
3. Install it (click *Next → Next → Finish*)

✅ Verify installation:

```bash
node -v
npm -v
```

You should see version numbers.

---

### **Step 2: Open Command Prompt / Terminal**

* **Windows:** Press `Win + R` → type `cmd` → Enter
* **Mac/Linux:** Open **Terminal**

---

### **Step 3: Install n8n Globally**

Run:

```bash
npm install -g n8n
```

⏳ Wait until installation completes.

Verify:

```bash
n8n --version
```

---

### **Step 4: Start n8n**

Run:

```bash
n8n
```

You should see:

```
Editor is now accessible at:
http://localhost:5678
```

---

### **Step 5: Open n8n in Browser**

Open your browser and go to:

```
http://localhost:5678
```

🎉 n8n is now running **locally, free, with no trial limits**.

---

### **Step 6: Stop n8n (When Needed)**

In Command Prompt / Terminal:

```
Ctrl + C
```

---

### **Step 7: Import Your Cloud Workflows**

1. Open n8n UI
2. Click **☰ Menu → Import workflow**
3. Upload your exported `.json` workflow files

---

### **Step 8: Reconnect Credentials**

* Re-add:

  * Google Sheets
  * Gmail
  * APIs
* (Cloud credentials do **not** transfer automatically)

---

### **Step 9: Keep n8n Running (Optional but Useful)**

#### Windows:

```bash
n8n start
```

#### Mac / Linux:

```bash
n8n start
```

(For production, PM2 is better, but this works.)

---

### **Step 10: Where n8n Data Is Stored**

* Workflows, creds, executions:

```
C:\Users\<your-username>\.n8n   (Windows)
~/.n8n                           (Mac/Linux)
```

---


