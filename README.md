# 💼 ExpenseFlow

<div align="center">
  <h3>🚀 Smart expense management with OCR receipt processing, multi-role dashboards, and automated workflows</h3>
  
  ![Next.js](https://img.shields.io/badge/Next.js-15-000000?style=for-the-badge&logo=next.js&logoColor=white)
  ![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black)
  ![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
  ![Tailwind](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
</div>

---

## ✨ Features

- 🔐 *Multi-role authentication* (Admin/Manager/Employee)
- 📸 *OCR receipt processing* with Tesseract.js
- 📧 *Email notifications* via SMTP with beautiful templates
- 💰 *Multi-currency support* with real-time conversion
- 🎨 *Dark/light theme toggle* with system preference
- ⚡ *Real-time expense tracking* and approval workflows

## 🚀 Quick Start

bash
# Clone the repository
git clone https://github.com/your-username/expense-Management-system.git
cd expense-Management-system

# Install dependencies
npm install

# Setup environment variables
cp .env.local.example .env.local
# Edit .env.local with your Gmail credentials (see below)

# Start development server
npm run dev


> 🌐 *Open* [http://localhost:3000](http://localhost:3000)

---

## ⚙ Environment Configuration

### 📄 Step 1: Create .env.local File

Copy the example file and edit it:

bash
cp .env.local.example .env.local


### 📧 Step 2: Configure Gmail SMTP

Edit your .env.local file with these *required* variables:

env
# 📧 SMTP Configuration for Gmail
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USER=your-email@gmail.com
SMTP_PASSWORD=your-16-character-app-password
SMTP_SECURE=false
SMTP_TLS=true
SMTP_FROM=your-email@gmail.com

# 📬 Email Configuration
FROM_EMAIL=your-email@gmail.com
FROM_NAME=ExpenseFlow

# 🔧 Debug Configuration (optional)
EMAIL_DEBUG=true


### 🔑 Step 3: Get Gmail App Password

> ⚠ *Important: You must use an **App Password*, not your regular Gmail password!

#### 3.1 Enable 2-Factor Authentication
1. Go to [Google Account Security](https://myaccount.google.com/security)
2. Click *"2-Step Verification"*
3. Follow the setup process (required for App Passwords)

#### 3.2 Generate App Password
1. Visit [App Passwords](https://myaccount.google.com/apppasswords)
2. Select app: *"Mail"*
3. Select device: *"Other (custom name)"* → Enter *"ExpenseFlow"*
4. Click *"Generate"*
5. 📋 *Copy the 16-character password* (format: xxxx xxxx xxxx xxxx)

#### 3.3 Update Your .env.local
Replace the placeholder values:

env
SMTP_USER=john.doe@gmail.com
SMTP_PASSWORD=abcd efgh ijkl mnop  # ← Your 16-character app password
SMTP_FROM=john.doe@gmail.com
FROM_EMAIL=john.doe@gmail.com


### ✅ Step 4: Test Email Configuration

1. Start the development server: npm run dev
2. Login as *Admin* (👑 admin@company.com / admin123)
3. Navigate to *"Email Configuration"* section
4. Click *"Test SMTP Connection"* button
5. Send a test email to verify setup

---

## 🔑 Default Login Credentials

| Role | Email | Password | Access |
|------|-------|----------|--------|
| 👑 *Admin* | admin@company.com | admin123 | Full system access |
| 👨💼 *Manager* | manager@company.com | manager123 | Approve/reject expenses |
| 👤 *Employee* | employee@company.com | employee123 | Submit expenses |

---

## 🛠 Available Scripts

bash
npm run dev      # 🔥 Start development server
npm run build    # 📦 Build for production
npm run start    # 🚀 Start production server
npm run lint     # 🔍 Run code linting


---

## 🚨 Troubleshooting

### 📧 Email Issues

*❌ Authentication Failed:*
- ✅ Use *App Password*, not regular Gmail password
- ✅ Verify 2FA is enabled on your Gmail account
- ✅ Double-check your Gmail address is correct
- ✅ Generate a new App Password if needed

*❌ Connection Timeout:*
- ✅ Check your internet connection
- ✅ Disable VPN/proxy temporarily
- ✅ Verify firewall isn't blocking port 587

*❌ Emails Not Received:*
- ✅ Check spam/junk folder
- ✅ Verify recipient email address
- ✅ Check Gmail sending limits (500 emails/day)

### 📸 OCR Issues

*❌ Poor Text Recognition:*
- ✅ Use clear, well-lit receipt images
- ✅ Ensure good contrast and avoid blur
- ✅ *Supported formats*: PNG, JPG, JPEG, PDF (max 10MB)

### 🔧 Development Issues

bash
# Clear cache and rebuild
rm -rf .next node_modules package-lock.json
npm install && npm run build


---

## 🔧 Tech Stack

- ⚛ *Frontend*: Next.js 15, React 19, TypeScript
- 🎨 *Styling*: Tailwind CSS, Radix UI
- 👁 *OCR*: Tesseract.js for receipt processing
- 📮 *Email*: Nodemailer with Gmail SMTP
- 📊 *Icons*: Lucide React

---

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details.

---

<div align="center">
  <p>🚀 <strong>Built with ❤ for efficient expense management</strong></p>
  <p>💼 Ready to streamline your expense workflows!</p>
</div>


member-  shreyansh pipaliya,kirtan ugreja,yugansh thacker
link- https://drive.google.com/drive/folders/1w8MJKa_H0qXecxUNa77JIIzLUs1TMSAv?usp=sharing
