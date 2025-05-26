# RealTimeCamera
🎯 Use Case: Real-Time Visual Prompting with Camera + LLM

🧠 Goal:

To interact with an AI model using your live webcam feed — by capturing frames and sending them (along with a prompt) to a backend (like OpenAI Vision or llava running locally) — and getting insightful, real-time responses.

⸻

💡 What This App Does

🔹 1. Captures Live Video Frames
	•	Accesses the user’s webcam
	•	Captures a frame at a configurable interval (100ms to 2s)

🔹 2. Sends Frames + Prompts to an LLM API
	•	Uses a POST request to /v1/chat/completions
	•	Payload includes:
	•	A textual instruction (e.g., “Describe this image”)
	•	A base64-encoded image from the camera feed

🔹 3. Displays AI-Generated Response
	•	Renders the AI’s interpretation of the scene
	•	Updates the response in real time
	•	Supports built-in prompt templates (e.g., Detect objects, Find anomalies) and custom prompts
