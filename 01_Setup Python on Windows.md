Setting up Python on Windows is a straightforward process. Here's a step-by-step guide:

---

### **Step 1: Download Python**
1. **Visit the Python website**: Go to [https://www.python.org/](https://www.python.org/).
2. **Download the installer**: Click on "Downloads" and choose the latest stable version for Windows (e.g., Python 3.x.x).

---

### **Step 2: Install Python**
1. **Run the installer**: Double-click the downloaded `.exe` file to start the installation.
2. **Select 'Add Python to PATH'**: Check the box **Add Python 3.x to PATH** at the bottom of the setup window. This is crucial to use Python from the command line.
3. **Choose 'Customize Installation' (Optional)**:
   - Leave all optional features selected (pip, IDLE, etc.).
   - Click **Next**.
4. **Customize install location**: By default, Python installs to `C:\Users\<YourUsername>\AppData\Local\Programs\Python\Python3x`. You can change this if needed.
5. **Install**: Click **Install Now** or **Install** to complete the installation.

---

### **Step 3: Verify Python Installation**
1. Open **Command Prompt**:
   - Press `Win + R`, type `cmd`, and press Enter.
2. Check the Python version:
   ```bash
   python --version
   ```
   This should display the installed Python version.
3. Check pip version:
   ```bash
   pip --version
   ```
   This verifies that the Python package manager is installed.

---

### **Step 4: Install a Code Editor (Optional)**
- Download **VS Code**: [https://code.visualstudio.com/](https://code.visualstudio.com/)
- Install the **Python extension** for syntax highlighting, debugging, and running scripts.

---

### **Step 5: Test Python**
1. Create a simple script:
   - Open Notepad or VS Code.
   - Write:
     ```python
     print("Hello, Python!")
     ```
   - Save the file as `test.py` in a folder.
2. Run the script:
   - Open Command Prompt.
   - Navigate to the folder:
     ```bash
     cd path\to\your\folder
     ```
   - Run the script:
     ```bash
     python test.py
     ```

You should see:
```plaintext
Hello, Python!
```

---

### **Step 6: (Optional) Install Useful Libraries**
Use pip to install libraries:
```bash
pip install numpy pandas matplotlib
```

Now you're ready to code in Python! Let me know if you face any issues.