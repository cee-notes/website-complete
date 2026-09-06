# CEE Mock Portal

A free online mock-test practice system for Medical Entrance (MBBS/BDS) exam preparation in Nepal, following the official MECEE-BL 2026 exam blueprint.

## 🌐 GitHub Pages Deployment

This application can now be hosted directly on GitHub Pages as a static web app with a built-in mock backend for preview/testing purposes.

### Quick Start

1. **Enable GitHub Pages:**
   - Go to your repository Settings → Pages
   - Under "Source", select `Deploy from a branch`
   - Choose branch: `main` (or `master`) and folder: `/ (root)`
   - Click Save

2. **Access Your Site:**
   - Your site will be available at: `https://<username>.github.io/<repository-name>/`
   - The site runs entirely in the browser using localStorage for data persistence

### Features

- **Student Mode:**
  - Register and log in (mock authentication)
  - Take mock exams with official MECEE-BL timing (54s per question)
  - Practice sessions with subject/difficulty filters
  - View results and analytics
  - Review past attempts

- **Teacher Mode:**
  - Approve/reject student registrations
  - Upload questions via CSV/XLSX bulk upload
  - Use PDF question builder
  - Add single questions manually
  - Generate daily model exams
  - View student progress reports

### Important Notes

⚠️ **GitHub Pages Version Limitations:**

This is a **preview/demo version** that runs entirely client-side with:
- Mock authentication (localStorage-based)
- Simulated backend (no real server)
- Local data persistence only (cleared if you clear browser data)
- No email notifications
- No multi-user synchronization

For the **full production version** with:
- Real user accounts and authentication
- Google Sheets database backend
- Email notifications
- Multi-user support with synchronization
- Persistent cloud storage

👉 Deploy to **Google Apps Script** using the `code.gs` file:
1. Create a new Google Sheet
2. Go to Extensions → Apps Script
3. Paste the entire `code.gs` content
4. Deploy as Web App (Execute as: Me, Who has access: Anyone)

### File Structure

```
├── index.html          # Complete frontend + mock backend (GitHub Pages)
├── code.gs             # Full Google Apps Script backend (production)
└── README.md           # This file
```

### Official Exam Blueprint

The mock tests follow the MECEE-BL 2026 official ratio:
- Zoology: 40 questions
- Botany: 40 questions
- Chemistry: 50 questions
- Physics: 50 questions
- MAT (Mental Agility Test): 20 questions
- **Total: 200 questions in 3 hours** (54 seconds per question)

### Technology Stack

- **Frontend:** Vanilla HTML/CSS/JavaScript (no frameworks)
- **Mock Backend:** In-browser JavaScript with localStorage
- **Production Backend:** Google Apps Script + Google Sheets + MailApp

### License

Free for educational use.

---

**Built for aspiring medical students in Nepal** 🇳🇵
