This application allows you to track flight deals for a list of cities stored in a Google Sheet (via Sheety). For each city, if the airport IATA code isn't specified, the program fetches it from the Amadeus API. Then, it searches for the cheapest flights within a given time range (e.g., tomorrow to six months from now). If a flight deal is found, it sends a WhatsApp message via Twilio.

Features
Integration with Google Sheets (Sheety)

Retrieves a list of destinations and their airport codes (if available).
Updates missing IATA codes automatically.
Flight Data Retrieval (Amadeus API)

Retrieves flight information using the Amadeus Flight Offers Search API (Test environment).
Identifies the cheapest available flight for each route.
Automated Notifications (Twilio)

Sends WhatsApp alerts for the best deals.
Customizable message content.
Environment Variable Management

Securely stores API keys and credentials using .env files and the python-dotenv package.
