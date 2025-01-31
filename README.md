# Summarizer
# Summary and Bullet Points Generation API

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repo-url>
   cd summary_api
   ```
2. Install dependencies:
  ```bash
  pip install -r requirements.txt
  ```
3. Set up environment variables:
  Create a .env file and add:
  ```
  GROQ_API_KEY=<your-api-key>
  ```
4. Apply migrations:
  ```
  python manage.py migrate
  ```
5. Run the server:
  ```
  python manage.py runserver
  ```

Usage
Authentication
Obtain an access token:

bash
```
curl -X POST http://127.0.0.1:8000/token/ -H "Content-Type: application/json" -d '{"username": "your_user", "password": "your_password"}'
```
Generate Summary
bash
```
curl -X POST http://127.0.0.1:8000/generate-summary/ -H "Authorization: Bearer <token>" -H "Content-Type: application/json" -d '{"text": "Your input text"}'
```
Generate Bullet Points
bash
```
curl -X POST http://127.0.0.1:8000/generate-bullet-points/ -H "Authorization: Bearer <
```
