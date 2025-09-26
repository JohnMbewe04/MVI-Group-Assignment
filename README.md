# Instructions to Run the Machine Vision & AI GUI

## 1. Set Up the Environment

1. Ensure you have **Python 3.11** installed (Anaconda recommended).

2. Create and activate a virtual environment:

   ```bash
   conda create -n mvi_env python=3.11 -y
   conda activate mvi_env
   ```

   *(If you already have an environment, you may skip creating a new one.)*

3. Install required libraries:

   ```bash
   pip install -r requirements.txt
   ```

---

## 2. Running the Breast Tumor AI Service

The breast tumor model is served separately through a FastAPI microservice. **You must start this before the GUI.**

1. Activate the **breast_env** virtual environment:

   ```bash
   conda activate breast_env
   ```

2. Navigate to the project folder where `breast_service.py` is located:

   ```bash
   cd path/to/project/folder
   ```

3. Start the service:

   ```bash
   python breast_service.py
   ```

   ⚠️ **Note:** You must be in the same folder as `breast_service.py` when running this command.

4. Once started, the service will be available at:

   ```
   http://127.0.0.1:8001
   ```

   Leave this terminal window running while you use the GUI.

---

## 3. Running the GUI

1. Open a new terminal.
2. Activate the main environment:

   ```bash
   conda activate mvi_env
   ```
3. Navigate to the project folder:

   ```bash
   cd path/to/project/folder
   ```
4. Run the GUI:

   ```bash
   python Assignment_GUI.py
   ```

---

## 4. Notes

* Ensure the `AI models/` folder and all `.keras`, `.h5`, `.pth`, and `.joblib` files are in the same project directory as the GUI code.
* The GUI will automatically detect models from these relative paths.
* Do **not** close the terminal running `breast_service.py` while using the GUI.
