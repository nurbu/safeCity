SafeCity
SafeCity is a web app that gives you a safer walking route by routing you around areas with high crime activity. Instead of just finding the fastest path, it looks at real NYC crime data and adjusts your route to avoid flagged spots.
We built this in 12 hours at a hackathon.

The Idea
Normal navigation apps don't think about safety — they just find the fastest route. In New York that can mean walking through some rough areas without even knowing it. We wanted to fix that by using actual crime data to inform how routes get calculated.

How the Routing Works
The core logic is pretty straightforward:

User enters a start point and destination
We load NYC crime data (pulled from a public dataset) and mark those locations on the map
We check each point along the suggested route — if it's flagged as a crime location, we reroute around it
We keep doing that until the path either avoids all crime points or gets as safe as it can be
The final route gets displayed on the map


Tech Stack

Next.js + TypeScript — frontend
Mapbox API — map rendering and routing
NYC crime dataset (public Excel data) — crime point data
CSS — styling


Running it locally
You'll need Node.js and a Mapbox API key.
bashgit clone https://github.com/nurbu/safeCity.git
cd safeCity
npm install
Create a .env.local file:
envNEXT_PUBLIC_MAPBOX_TOKEN=your_token_here
Then:
bashnpm run dev
Go to http://localhost:3000.

What we'd add with more time

Crime heatmap so you can see density, not just individual points
Weight routes by crime type or severity
Let users report incidents directly in the app
Support for cities outside NYC
Make it work better on mobile


Team
Built by a small team at a hackathon. Backend, routing logic, and Mapbox integration by @nurbu.
