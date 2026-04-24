🦾 ARIA – Accessible Routing & Intelligent Alerts
ARIA is an assistive navigation system designed for blind and visually impaired users. It combines voice interaction, Google Maps routing, risk detection, and vehicle alerts to ensure safe walking navigation in real‑world environments.

🚀 Features
Voice Interface

Listens to user commands (Speech‑to‑Text via Gemini).

Speaks navigation instructions (Text‑to‑Speech via Gemini).

Navigation

Uses Google Maps Directions API to fetch walking routes.

Provides step‑by‑step spoken instructions.

Society Risk Alerts

Collects inputs from nearby people (potholes, construction, crowds).

Warns users about hazards in real time.

Risk Engine

Analyzes route steps + society alerts.

Detects dangerous conditions and generates warnings.

Vehicle Alerts

Uses Firebase Cloud Messaging (FCM) to notify nearby vehicles about pedestrians and risks.

🔑 API Keys
Set your API keys in the code before running:

python
GOOGLE_MAPS_API_KEY = "GOOGLE_MAPS_KEY"
GEMINI_API_KEY = "GOOGLE_GEMINI_KEY"
FIREBASE_SERVER_KEY = "FIREBASE_KEY"
📂 Project Structure
Code
voice_interface.py   # Handles listening & speaking
maps_navigation.py   # Fetches walking routes
society_inputs.py    # Collects alerts from people nearby
risk_engine.py       # Analyzes risks
vehicle_alerts.py    # Sends alerts to vehicles
main.py              # Runs ARIA end-to-end
▶️ Usage
Run the main script:

bash
python main.py
Example flow:

Blind user says: “Navigate me to the nearest hospital”

ARIA fetches walking route via Google Maps.

ARIA speaks each step aloud.

Society alerts are checked for risks.

ARIA warns the user and notifies vehicles if needed.

User reaches destination safely.

🛠️ Tech Stack
Google Maps API – Routing & navigation

Gemini API – Speech‑to‑Text & Text‑to‑Speech

Firebase Cloud Messaging (FCM) – Vehicle alerts

Python – Core implementation

🌍 Vision
ARIA aims to make urban navigation safer for blind and visually impaired users by combining AI, crowdsourced alerts, and real‑time communication with vehicles.
