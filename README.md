# AI Travel Guide

AI-powered travel guide that generates historical descriptions and Murf AI audio guides in multiple languages and voices.

## Project Structure
- `Frontend/` - static HTML/CSS/JavaScript frontend
- `Backend/` - Flask API for Gemini-generated descriptions and Murf audio

## Local Setup
1. Create a Python virtual environment in `Backend/`.
2. Install dependencies: `pip install -r requirements.txt`
3. Create `Backend/.env` from `.env.example` and add your own API keys.
4. Set the frontend API URL in `Frontend/index.js` to your backend URL.
5. Run `python app.py`.

## Deployment
- Backend: Render Web Service, root directory `Backend`, build command `pip install -r requirements.txt`, start command `gunicorn app:app`.
- Frontend: Vercel static deployment, root directory `Frontend`.
- Keep API keys only in Render environment variables; never commit `.env` or secret values.
