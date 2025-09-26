# 📋 Instructions to Run the GUI

### 1. Install Python

Make sure you have **Python 3.10 or later** installed.
Check with:

```bash
python --version
```

---

### 2. Create a Virtual Environment

Open a terminal/command prompt inside this project folder and run:

**Windows:**

```bash
python -m venv venv
venv\Scripts\activate
```

**Mac/Linux:**

```bash
python3 -m venv venv
source venv/bin/activate
```

---

### 3. Install Dependencies

Once the environment is activated, install all required libraries:

```bash
pip install -r requirements.txt
```

---

### 4. Run the Application

Now you can launch the GUI by running:

```bash
python gui_app.py
```

---

### 5. Notes

* All **AI models** are located in the `models/` subfolders. Do **not** rename or move them, otherwise the GUI may not find them.
* If you face an error like `ModuleNotFoundError`, make sure your virtual environment is **activated** before running the GUI.
* To deactivate the environment when done:

```bash
deactivate
```

---
