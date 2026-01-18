
# University Computer Science Department Website

A professional, fully containerized, and automatically deployed departmental website implementing complete DevOps practices including **Git Flow, CI/CD pipelines, Docker containerization**, and **multi-environment deployment**.

---

## 📋 Project Overview

This project demonstrates a complete end-to-end DevOps workflow by building a **static website for a Computer Science Department**.

The website is containerized using **Docker** and automatically deployed to three separate environments:

* **Development**
* **Staging/QA**
* **Production**

All deployments are handled using **GitHub Actions CI/CD pipelines**.

---

## Key Features

* **🎨 Responsive Design:** Mobile-friendly, modern UI
* **🐳 Docker Containerization:** Optimized multi-stage Dockerfile
* **🔄 Git Flow Workflow:** Proper branching strategy
* **🚀 CI/CD Pipelines:** Automated testing, building, and deployment
* **🔒 Secrets Management:** GitHub Environments with protected secrets
* **📦 Multi-Environment Deployment:** Dev, Staging, and Production
* **✅ Code Quality:** HTML/CSS linting and validation

---

## 🏗️ Project Structure

```
University-Department-Website/
├── src/                  # Source files
│   ├── index.html        # Home page
│   ├── courses.html      # Courses page
│   ├── faculty.html      # Faculty page
│   ├── admissions.html   # Admissions page
│   ├── contact.html      # Contact page
│   └── styles/
│       └── style.css     # Shared stylesheet
├── .github/workflows/    # GitHub Actions workflows
│   ├── Linting.yml       # CI pipeline (lint & build)
│   ├── cd-dev.yml        # CD for development
│   ├── cd-staging.yml    # CD for staging/QA
│   └── cd-prod.yml       # CD for production
├── Dockerfile            # Docker image definition
├── nginx.conf            # Nginx web server config
├── .gitignore            # Git ignore rules
└── README.md             # This file
```

---

## 📄 Web Pages

### Home Page (`index.html`)

* Department overview and mission statement
* Key highlights and achievements
* Quick navigation to other sections
* Hero banner with call-to-action

### Courses Page (`courses.html`)

* Core, advanced, and elective courses
* Course descriptions and availability
* Registration information
* Prerequisites and credit hours

### Faculty Page (`faculty.html`)

* Faculty member profiles
* Specializations and research areas
* Office hours and contact information
* Research focus areas

### Admissions Page (`admissions.html`)

* Bachelor's and Master's programs
* Admission criteria and requirements
* Application process timeline
* Important deadlines
* Tuition and financial aid information

### Contact Page (`contact.html`)

* Contact information and office details
* Contact form
* Quick links
* Google Maps integration
* Office hours

---

## 🔄 Git Flow Strategy

**Branch Structure:**

* **main:** Production-ready code (Protected)
* **release/:** Release candidates (e.g., `release/v1.0.0`)
* **develop:** Development branch (Protected)
* **feature/:** Feature branches (e.g., `feature/new-page`)
* **bugfix/:** Bug fix branches (e.g., `bugfix/homepage-styling`)
* **hotfix/:** Hotfix branches (e.g., `hotfix/critical-bug`)

-----------------------------------------------------------------------------

## 🚀 Run Everything Locally

```bash
git clone https://github.com/umairakhtar0/department-web.git
npm install 
npx htmlhint "**/*.html"
npx stylelint "src/styles/**/*.css"
```

---------------------------------------------------------------------

## 🟢 Push to GitHub

```bash
git add .
git commit -m "MESSAGE"
git checkout -b BRANCHNAME
git add .
git commit -m "MESSAGES"
git push origin branchname
```

* Make a **Pull Request (PR)** on GitHub to the `develop` branch.
* GitHub Actions will **run automatically** for linting, building, and deployment.

-------------------------------------------------------------------------------------------

