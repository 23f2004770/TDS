# Vehicle Parking Application 🚗

The **Vehicle Parking Application** is a web-based system designed to manage parking lots, user bookings, and provide insightful analytics for both users and administrators. It allows users to book and release parking spots, track their parking history, and manage profiles, while administrators can manage lots, monitor spot usage, and view summary reports in visual form.

---

## 🚀 Features

### 👤 User Features
- 🔍 **Book Parking Lot**: Users can book a spot in available parking lots.
- 🆓 **Release Functionality**: Release a spot after use; ensures proper status tracking.
- 📊 **User Summary**: Users can view their own parking usage data with charts.
- ✏️ **Edit Profile**: Users can update email, password, and username.

### 🛠️ Admin Features
- 👥 **User Management**: Delete users (only after spot is released).
- 🅿️ **Parking Lot Management**: Add, edit, or delete parking lots and spots.
- 📈 **Summary Reports**: View analytics on revenue, usage, and spot status (pie/bar charts).
- 🧑‍💼 **Edit Profile**: Admins can update their login credentials and info.

---

## 🧰 Technologies Used

| Layer        | Stack                                 |
|--------------|----------------------------------------|
| **Backend**  | Flask (Python)                         |
| **Frontend** | HTML, CSS, Bootstrap, Jinja2 Templates |
| **Database** | SQLAlchemy with SQLite                 |
| **Charts**   | Matplotlib                             |
| **Auth**     | Flask-Login                            |

---

## ⚙️ Installation

### 1. Fork and Clone
```bash
git clone https://github.com/YOUR-USERNAME/vehicle_parking_app.git
cd vehicle_parking_app
```

###2. Create Virtual Environment
```bash
python -m venv .venv
.venv\Scripts\activate  # On Windows
# or
source .venv/bin/activate  # On macOS/Linux
```
###3. Install Dependencies
```bash
pip install -r requirements.txt
```
##4. Run the Application
```bash
python app.py
```
```bash
Visit http://127.0.0.1:5000/ in your browser.
```
###Project Structure
```bash
parking_app_23f2004770/
│
├── controllers/                  # Route definitions
│   ├── auth.py                   # Login and registration routes
│   └── main.py                   # Admin and user route handling
│
├── static/                       # Static files
│   ├── images/                   # Chart images (bar/pie)
│   └── img/                      # Login/Register page images
│
├── templates/                    # HTML templates (Jinja2)
│   ├── index.html                       # Landing/Home page
│   ├── login.html                       # Login form
│   ├── register.html                    # Registration form
│   ├── admin_dashboard.html            # Admin dashboard
│   ├── user_dashboard.html             # User dashboard
│   ├── add_parking_lot.html            # Add new parking lot
│   ├── edit_parking_lot.html           # Edit existing parking lot
│   ├── view_parking_spot.html          # View a specific spot
│   ├── view_parking_spots_by_lot.html  # All spots for a lot
│   ├── occupied_parking_details.html   # Occupied spot details
│   ├── parking_spot_details.html       # Spot usage info
│   ├── registered_users.html           # Admin - user management
│   ├── admin_edit_profile.html         # Admin profile update
│   ├── user_edit_profile.html          # User profile update
│   ├── admin_summary.html              # Admin analytics summary
│   ├── user_summary.html               # User analytics summary
│
├── models.py                    # Database models
```
├── app.py                       # Main app entry point
├── config.py (if present)       # Configuration (if used)
├── requirements.txt             # Python dependencies
├── .gitignore                   # Files to ignore in Git
├── README.md                    # You're reading it!
