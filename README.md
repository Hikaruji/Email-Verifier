# Email-Verifier
Use to check whether email still active or not 

This is a local cold email verification tool. Drag in a CSV and it will:
- Validate each email live (MX, SMTP, syntax)
- Show real-time progress per file
- Let you cancel jobs mid-run
- Persist your results even after refresh
- Let you download the verified leads when ready

---
## 🧱 Setup

1. Create a folder called:
```
Verify
```

2. Drag in these files:
- `verify-app.py`
- `index.html`
- Your test CSV (e.g. `Testleads.csv`)

---

## ⚙️ Install Dependencies

Open Terminal, then run:

```python -m venv venv
venv\Scripts\activate
pip install flask flask-cors dnspython
```

---

## 🚀 Run the App

### Terminal Tab 1:
```
venv\Scripts\activate
python verify-app.py

```
You should see:
```
🔥 VERIFIER RUNNING 🔥
```

### Terminal Tab 2:
```cd "C:\Users\YourName\Desktop\Verify"
python -m http.server 3000

```

---

## 🌐 Use the Tool

Open in your browser:
```
http://localhost:3000/index.html
```

- Drag in one or more CSVs
- Each file shows a progress bar, live email log, cancel button, and close (X)
- When done, a download link will appear
- Everything persists across refreshes

---
