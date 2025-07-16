# Docker Compose Usage — Flask Calculator API

## 🐳 How to Build and Run the App

bash
docker compose up --build

This builds the Docker image and runs the Flask API container.

⸻

🔬 How to Test the API

Use this PowerShell command:

curl -Uri "http://localhost:5000/add" -Method POST -Body '{"num1":6,"num2":7}' -ContentType "application/json"

✅ Expected Output:

{
  "result": 13.0
}


⸻

🛑 How to Stop and Clean

To stop the container:

CTRL+C

Then to clean up everything:

docker compose down

---

