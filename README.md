# CropBazaar

CropBazaar - Your Crop, Right Mandi, Right Time.

CropBazaar is an AI-powered agricultural market intelligence platform. This repository contains the initial frontend and backend setup; application features will be added in later steps.

## Project Structure

```text
frontend/  React + Vite + Tailwind CSS client
backend/   FastAPI service
data/      Data files and processing inputs
ml/        Machine learning code and artifacts
```

## Run the Frontend

```bash
cd frontend
npm install
npm run dev
```

Open the local URL printed by Vite, usually `http://localhost:5173`.

## Run the Backend

From the repository root, create and activate a virtual environment:

```bash
cd backend
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
uvicorn main:app --reload --port 8000
```

The health endpoint is available at `http://localhost:8000/api/health`.

## Initial Checks

With the backend running, verify:

```bash
curl http://localhost:8000/api/health
```

Expected response:

```json
{"status":"ok"}
```

The frontend and backend run independently. No dashboard, mock data, ML model, authentication, or database is included yet.
