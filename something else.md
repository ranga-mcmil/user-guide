# POTRAZ Portal

A comprehensive self-service web portal for the **Postal and Telecommunications Regulatory Authority of Zimbabwe (POTRAZ)**. This Django-based application enables individuals and organizations to apply for, manage, and renew various telecommunications and postal service licenses in Zimbabwe.

## 🚀 Features

### User Management
- **Dual Account Types**: Individual and Organization/Company registration
- **Email-based Authentication**: Secure login using email addresses
- **Phone Verification**: SMS-based OTP verification using Twilio
- **Business Partner Integration**: Automatic BP number generation for SAP integration

### License Management
- **Multi-step Application Wizards**: Streamlined application process for different license types
- **License Tracking**: View, update, and renew existing applications
- **Document Management**: Upload and manage required documents
- **Status Notifications**: Email and SMS notifications for application updates

### License Categories

#### 📡 Telecommunications Licenses
- ISP (Internet Service Provider) License
- Unified Telecommunication License
- Telecommunication Network Services License
- Network Facilities License
- Application Services License
- Inter Gateway Service License
- Mobile Virtual Network License

#### 📮 Postal and Courier Services
- Postal (General) Services License
- Commercial International/Regional/Domestic Courier Services
- Inter-city and Intra-city Courier Services
- Various classes of courier services

#### 🔧 Specialized Licenses
- Short Code and Numbering Allocation
- Rural Fixed Broadband Wireless
- Private Network License
- Earth Station License
- Fixed Wireless Access
- Radio Relay/Point to Point
- Mobile Satellite Station
- Private Radio Transceiver
- Satellite Landing Rights
- Dealership License
- Equipment Type Approval License

## 🛠️ Technology Stack

- **Backend**: Django 5.0.2
- **Database**: MySQL
- **Frontend**: Bootstrap, HTML5, CSS3, JavaScript
- **SMS Service**: Twilio
- **PDF Generation**: WeasyPrint
- **Email Service**: Office 365 SMTP
- **File Storage**: Local media storage
- **Backend Integration**: SAP system integration

## 📋 Prerequisites

- Python 3.13+
- MySQL 5.7+
- Virtual environment (recommended)

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd potraz-portal
   ```

2. **Create and activate virtual environment**
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Environment Configuration**
   Create a `.env` file in the project root with the following variables:
   ```env
   SECRET_KEY=your-secret-key-here
   TWILIO_ACCOUNT_SID=your-twilio-account-sid
   TWILIO_AUTH_TOKEN=your-twilio-auth-token
   BASE_URL=your-base-url
   BACKEND_URL_QAS=your-sap-backend-url
   SAP_CLIENT_QAS=your-sap-client
   ```

5. **Database Setup**
   ```bash
   # Create MySQL database
   mysql -u root -p
   CREATE DATABASE potraz_db;
   CREATE USER 'potraz_user'@'localhost' IDENTIFIED BY 'Pa$$word';
   GRANT ALL PRIVILEGES ON potraz_db.* TO 'potraz_user'@'localhost';
   FLUSH PRIVILEGES;
   ```

6. **Run Migrations**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

7. **Create Superuser**
   ```bash
   python manage.py createsuperuser
   ```

8. **Run Development Server**
   ```bash
   python manage.py runserver
   ```

## 📁 Project Structure

```
potraz-portal/
├── accounts/                 # User management app
├── core/                    # Core utilities and helpers
├── dashboard/               # Main dashboard functionality
├── downloads/               # File download management
├── emails/                  # Email templates and utilities
├── errors/                  # Custom error pages
├── licences/                # License management app
│   ├── forms/              # License application forms
│   ├── templates/          # License-related templates
│   └── views/              # License views and wizards
├── potraz_portal/          # Main project settings
├── repositories/           # Data access layer
├── shortcodes/             # Short code management
├── static_files/           # Static assets (CSS, JS, images)
├── templates/              # Base templates
└── utils/                  # Utility functions and constants
```

## 🔧 Configuration

### Database Configuration
The application is configured to use MySQL by default. Update `settings.py` if you need to use a different database:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'potraz_db',
        'USER': 'potraz_user',
        'PASSWORD': 'Pa$$word',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

### Email Configuration
Email settings are configured for Office 365. Update the following in `settings.py`:

```python
EMAIL_HOST = "smtp.office365.com"
EMAIL_PORT = 587
EMAIL_HOST_USER = "noreply@potraz.zw"
EMAIL_USE_TLS = True
```

### SMS Configuration
Twilio integration for SMS notifications:

```python
TWILIO_ACCOUNT_SID = env('TWILIO_ACCOUNT_SID')
TWILIO_AUTH_TOKEN = env('TWILIO_AUTH_TOKEN')
```

## 🚀 Usage

### For End Users

1. **Registration**
   - Visit the portal and choose between Individual or Organization registration
   - Complete the registration form with required details
   - Verify your phone number via SMS

2. **License Application**
   - Log in to your account
   - Navigate to the desired license category
   - Complete the multi-step application wizard
   - Upload required documents
   - Submit your application

3. **Application Management**
   - View all your applications in the dashboard
   - Track application status
   - Update existing applications
   - Renew licenses when needed

### For Administrators

1. **Access Admin Panel**
   - Navigate to `/admin/`
   - Log in with superuser credentials

2. **Manage Applications**
   - Review submitted applications
   - Update application statuses
   - Manage user accounts

## 🔒 Security Features

- **CSRF Protection**: Built-in Django CSRF protection
- **Authentication**: Secure email-based authentication
- **Phone Verification**: SMS-based OTP verification
- **File Upload Security**: Validated file uploads
- **Environment Variables**: Sensitive data stored in environment variables

## 📱 API Integration

The portal integrates with:
- **SAP Backend**: For business process management
- **Twilio**: For SMS notifications
- **Office 365**: For email services

## 🐛 Troubleshooting

### Common Issues

1. **Database Connection Error**
   - Ensure MySQL is running
   - Verify database credentials in settings.py
   - Check if the database exists

2. **SMS Not Working**
   - Verify Twilio credentials in environment variables
   - Check Twilio account balance
   - Ensure phone numbers are in correct format

3. **Email Not Sending**
   - Verify Office 365 credentials
   - Check SMTP settings
   - Ensure firewall allows SMTP traffic

## 📝 License

This project is proprietary software developed for POTRAZ (Postal and Telecommunications Regulatory Authority of Zimbabwe).

## 🤝 Contributing

This is an internal project for POTRAZ. For contributions or issues, please contact the development team.

## 📞 Support

For technical support or questions about the portal, please contact:
- **Email**: noreply@potraz.zw
- **Organization**: POTRAZ (Postal and Telecommunications Regulatory Authority of Zimbabwe)

---

**Note**: This portal is designed specifically for Zimbabwe's telecommunications and postal regulatory environment. Ensure compliance with local regulations when using this system.
