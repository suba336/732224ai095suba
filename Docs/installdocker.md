---

### **Step 1: Check system requirements**

1. Windows 10/11 (64-bit)
2. WSL 2 supported (most modern systems are)

---

### **Step 2: Download Docker Desktop**

1. Go to 👉 **[https://www.docker.com/products/docker-desktop](https://www.docker.com/products/docker-desktop)**
2. Click **Download for Windows**

---

### **Step 3: Run the installer**

1. Double-click the downloaded `.exe`
2. Keep these **checked**:

   * ✅ Use WSL 2 instead of Hyper-V
   * ✅ Add shortcut to desktop
3. Click **OK → Install**

---

### **Step 4: Restart your computer**

🚨 Important — Docker won’t work properly without this.

---

### **Step 5: Start Docker Desktop**

1. Open **Docker Desktop**
2. Wait until it says **“Docker is running”**

---

### **Step 6: Verify Docker installation**

Open **Command Prompt / PowerShell**:

```bash
docker --version
```

You should see:

```
Docker version xx.xx.x
```

Optional test:

```bash
docker run hello-world
```

If you see a success message → Docker is working 🎉

---

