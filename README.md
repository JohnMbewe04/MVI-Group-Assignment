# Instructions for Running the Machine Vision & AI System

## 1. Install Python

* Make sure you have **Python 3.10** installed (recommended).

  > Note: Some models may not work properly on Python 3.11+

Download: [https://www.python.org/downloads/release/python-3100/](https://www.python.org/downloads/release/python-3100/)

---

## 2. Set Up a Virtual Environment

Open a terminal in the project folder and run:

```bash
python -m venv venv
```

Activate the environment:

* **Windows (CMD):**

  ```bash
  venv\Scripts\activate
  ```
* **Windows (PowerShell):**

  ```powershell
  .\venv\Scripts\activate
  ```
* **Mac/Linux:**

  ```bash
  source venv/bin/activate
  ```

---

## 3. Install Required Libraries

Install all dependencies from the provided `requirements.txt`:

```bash
pip install -r requirements.txt
```

---

## 4. Start the Breast Tumor Microservice

The **Breast Tumor AI model** runs in its own microservice.
While the virtual environment is active, run:

```bash
python breast_service.py
```

* Leave this terminal running.
* It will start a server at **[http://127.0.0.1:8001](http://127.0.0.1:8001)**.
* Do **not** close this window while using the GUI.

---

## 5. Run the GUI

Open **another terminal**, activate the virtual environment again, and run:

```bash
python gui.py
```

This will launch the **Machine Vision & AI System GUI**.

---

## 6. Using the System

* You can test different subsystems:

  * **Machine Vision:** Rule-based X-ray, Fundus, MRI, Breast tumor detection
  * **AI Models:** Deep learning models for Chest X-ray, Brain MRI, Fundus, Breast tumor

* For **Breast Tumor AI**, ensure `breast_service.py` is running (step 4).

---

✅ That’s it! You’re ready to use the system.
⚠️ If you encounter errors, double-check:

* You are using **Python 3.10**
* You installed all requirements
* The **microservice is running** for breast tumor AI

---
