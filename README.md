# Django-4.x-ORM

#Steps To execute this project

### **1. Activate Virtual Environment (If Not Already)**
Before installing dependencies, it's best to work in a virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate  # On macOS/Linux
venv\Scripts\activate     # On Windows (PowerShell)
```

### **2. Install Dependencies**
Since you already ran:
```bash
pip install -r requirements.txt
```
Ensure it completed successfully. If there were dependency issues, try:
```bash
pip install --upgrade --force-reinstall -r requirements.txt
```

### **3. Check Django Version**
Ensure you are using the installed Django version (4.0.6):
```bash
python -m django --version
```
If it's still showing Django 5.x, you might be in the wrong environment.

### **4. Apply Migrations**
Run the following command to set up your database:
```bash
python manage.py migrate
```

### **5. Create Superuser (Optional)**
If you need an admin account, create one:
```bash
python manage.py createsuperuser
```

### **6. Run the Development Server**
Finally, start the Django server:
```bash
python manage.py runserver
```
Now visit Admin **http://127.0.0.1:8000/admin** in your browser.
Now visit page **http://127.0.0.1:8000/query/ex1/** in your browser.

### **Troubleshooting**
- If `python manage.py runserver` fails, check `settings.py` for database issues.
- If static files aren’t loading, run:
  ```bash
  python manage.py collectstatic
  ```
- If you see `ModuleNotFoundError`, reinstall missing dependencies with:
  ```bash
  pip install -r requirements.txt
  ```

Let me know if you run into any issues! 🚀