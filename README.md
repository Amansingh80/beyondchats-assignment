# BeyondChats Full-Stack Developer Assignment

A comprehensive full-stack project demonstrating web scraping, CRUD APIs, LLM integration, and modern frontend development.

## 📋 Assignment Overview

This project is a technical assignment for a Full-Time Remote Developer position at BeyondChats, showcasing skills in:
- **Laravel** (Backend API)
- **NodeJS** (LLM-based content optimization)
- **ReactJS** (Frontend UI)

## 🎯 Project Phases

### Phase 1: Laravel Backend (Moderate Difficulty)
- Scrape 5 oldest articles from [BeyondChats Blogs](https://beyondchats.com/blogs/)
- Store articles in database
- Create CRUD APIs for article management

### Phase 2: NodeJS LLM Script (Very Difficult)
- Fetch latest article from Laravel API
- Search article title on Google
- Scrape top 2 blog/article results
- Use LLM API to optimize original article based on top-ranking content
- Publish updated article via CRUD APIs
- Add citations for reference articles

### Phase 3: ReactJS Frontend (Very Easy)
- Fetch articles from Laravel APIs
- Display original and updated articles
- Responsive, professional UI design

## 🚀 Quick Start

### Prerequisites
- PHP >= 8.1
- Composer
- Node.js >= 18.x
- MySQL/PostgreSQL
- npm/yarn

### Installation

```bash
# Clone repository
git clone https://github.com/Amansingh80/beyondchats-assignment.git
cd beyondchats-assignment

# Backend setup (Laravel)
cd backend
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve

# NodeJS script setup
cd ../nodejs-script
npm install
cp .env.example .env
node index.js

# Frontend setup (ReactJS)
cd ../frontend
npm install
npm start
```

## 📁 Project Structure

```
beyondchats-assignment/
├── assignment/              # Assignment documentation
├── backend/                 # Laravel API
│   ├── app/
│   ├── database/
│   └── routes/
├── nodejs-script/           # LLM optimization script
│   ├── src/
│   └── package.json
├── frontend/                # ReactJS application
│   ├── src/
│   └── package.json
└── README.md
```

## 🔧 Tech Stack

- **Backend**: Laravel 10.x, MySQL
- **Script**: Node.js, Puppeteer/Cheerio, OpenAI/Anthropic API
- **Frontend**: React 18.x, Axios, TailwindCSS
- **Tools**: Git, Composer, npm

## 📊 Architecture Diagram

```
┌─────────────────┐
│  BeyondChats    │
│  Blog Website   │
└────────┬────────┘
         │ Scrape
         ▼
┌─────────────────┐      ┌──────────────┐
│  Laravel API    │◄─────┤  MySQL DB    │
│  (CRUD)         │      └──────────────┘
└────────┬────────┘
         │ API Calls
         ▼
┌─────────────────┐      ┌──────────────┐
│  NodeJS Script  │─────►│  Google      │
│  (LLM)          │      │  Search      │
└────────┬────────┘      └──────────────┘
         │                      │
         │                      ▼
         │               ┌──────────────┐
         └──────────────►│  LLM API     │
                         └──────────────┘
                                │
                                ▼
                         ┌──────────────┐
                         │  ReactJS UI  │
                         └──────────────┘
```

## 🌐 Live Demo

**Frontend**: [Coming Soon]

## 📝 API Endpoints

### Articles
- `GET /api/articles` - List all articles
- `GET /api/articles/{id}` - Get single article
- `POST /api/articles` - Create article
- `PUT /api/articles/{id}` - Update article
- `DELETE /api/articles/{id}` - Delete article

## ⏰ Timeline

- **Due Date**: Thursday, 25 December 2024, 11:59 PM IST
- **Time Allocation**: 6-8 hours

## 📈 Evaluation Criteria

- ✅ Completeness: 50%
- ✅ README & Setup Docs: 25%
- ✅ Live Link: 15%
- ✅ Code Quality: 10%

## 📄 License

This code is the property of the author and is submitted for employment evaluation purposes only.

## 👤 Author

**Anuj Singh**
- GitHub: [@Amansingh80](https://github.com/Amansingh80)
- Email: kidmada2025@gmail.com

## 🙏 Acknowledgments

Assignment provided by [BeyondChats](https://beyondchats.com)

---

**Note**: Partial completion is acceptable. This project demonstrates problem-solving approach, hands-on expertise, and engineering judgment under time constraints.