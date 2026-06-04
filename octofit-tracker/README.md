# OctoFit Tracker

A modern multi-tier fitness tracking application built with React 19, Express.js, TypeScript, and MongoDB.

## Project Structure

```
octofit-tracker/
├── frontend/          # React 19 + Vite
│   ├── src/
│   ├── package.json
│   ├── vite.config.js
│   └── index.html
└── backend/           # Node.js + Express + TypeScript + Mongoose
    ├── src/
    ├── package.json
    ├── tsconfig.json
    └── .env.example
```

## Technology Stack

### Frontend
- **React 19**
- **Vite** (Build tool)
- **Port:** 5173

### Backend
- **Node.js**
- **Express.js**
- **TypeScript**
- **Mongoose** (MongoDB ODM)
- **Port:** 8000

### Database
- **MongoDB**
- **Port:** 27017

## Getting Started

### Prerequisites
- Node.js 18+
- MongoDB running locally or accessible

### Frontend Setup

```bash
cd octofit-tracker/frontend
npm install
npm run dev
```

The frontend will be available at `http://localhost:5173`

### Backend Setup

```bash
cd octofit-tracker/backend
npm install
cp .env.example .env
npm run dev
```

The backend will be available at `http://localhost:8000`

### Verify Backend Connection

```bash
curl http://localhost:8000/api/health
```

## Development Commands

### Frontend
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

### Backend
- `npm run dev` - Start development server
- `npm run build` - Build TypeScript
- `npm start` - Run compiled JavaScript

## Port Configuration

| Service | Port | Environment |
|---------|------|-------------|
| Frontend (Vite) | 5173 | `vite.config.js` |
| Backend (Express) | 8000 | `backend/src/index.ts` |
| MongoDB | 27017 | `backend/src/index.ts` |

## Next Steps

1. Define MongoDB schemas using Mongoose
2. Create API routes and controllers
3. Implement authentication
4. Build React components and pages
5. Connect frontend to backend API
