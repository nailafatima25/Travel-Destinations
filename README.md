Readme · ✈️ Travel-Destination Explorer & Itinerary Planner — Browse & Save Travel Destinations with Itineraries


A front-end web application to browse popular travel destinations, fully interactive travel destination explorer — browse 12 handpicked destinations, filter by vibe, view 3-day itineraries, and save your favorites. No login. No backend. Just open and explore.

🔗 Live Demo → https://nailafatima25.github.io/Travel-Destinations/

✨ Highlights

🗺️ 12 curated destinations — Tokyo, Paris, Bali, Maldives, NYC, and more

🏷️ Filter by category — Couple, Adventure, Budget, Family, Shopping, Relaxation, and more

🔍 Live search — Instantly filter by destination name, country, vibe, or description

📅 3-day itineraries — Tap any card to view a detailed day-by-day plan in a modal popup

🔖 Save destinations — Bookmarked picks persist in your browser using localStorage

📱 Fully responsive — Works beautifully on desktop, tablet, and mobile


📖 Overview
Travel Picks is a front-end web application that helps travelers quickly discover and organize destination ideas. Many travel websites are cluttered, slow, or require sign-ups just to browse. This project solves that by offering a clean, fast, and zero-friction browsing experience, entirely in the browser, with no backend or account needed.
The app was built from scratch using only HTML, CSS, and vanilla JavaScript, no frameworks, no libraries. The goal was to demonstrate how far core web technologies can go when paired with thoughtful design. Each destination card includes a country tag, category badges, a short description, best travel time, and vibe summary. Clicking "View Itinerary" opens a polished modal with a 3-day activity breakdown and quick travel tips.
One of the more interesting technical challenges was building the save/unsave system using the browser's localStorage API so that bookmarked destinations persist between sessions without any database. Another challenge was making the search and filter work together in real time, both the tab filter and the text search needed to compose cleanly without conflicts, which required careful state management in plain JavaScript.
Future improvements I'd love to add include a map view using the Google Maps or Leaflet API, a cost estimator per destination, user-submitted reviews, and a trip planner where you can drag and reorder your saved destinations into a full itinerary. I also plan to expand the destination list and add animated card transitions for a more polished feel.

👤 Author
Naila Fatima

🌐 Live Site
💻 GitHub


🎬 Demo

📽️ 

Screenshots:
Destination GridItinerary Modal


🛠️ Tools & Technologies
TechnologyPurposeHTML5Page structure and semantic markup CSS Styling, responsive grid, animationsJavaScript search, modal, localStorageGoogle FontsTypography — Playfair Display

🚀 How to Install & Run Locally
No dependencies or build tools needed — this is a pure HTML/CSS/JS project.
Step 1: Clone the repository
bashgit clone https://github.com/nailafatima25/Travel-Destinations.git
Step 2: Navigate into the folder
bashcd Travel-Destinations
Step 3: Open in your browser
bashopen index.html
Or simply double-click index.html in your file explorer — it opens directly in any browser.

🧭 How to Use

Browse — Scroll through the destination cards on the main grid
Filter — Click any tab (e.g. "Couple", "Budget", "Adventure") to narrow results
Search — Type in the search bar to filter by name, country, or vibe
View Itinerary — Click the gold "View Itinerary" button on any card to open a 3-day plan
Save — Click "Save" to bookmark a destination; it appears in the "Saved Destinations" section below
Remove — In the Saved section, click "Remove" to delete a bookmark


🗂️ Project Structure
Travel-Destinations

├── index.html       ← All HTML, CSS, and JavaScript in one file

└── README.md        ← You are here

🐛 Bugs Fixed

Save button state out of sync — After saving from the modal, the card button in the grid wasn't updating to "✓ Saved" until a full re-render was triggered. Fixed by calling render() after every save/unsave action to keep all UI in sync.
Search + filter conflict — Early versions broke when a user had both a search query typed and a category tab active. Fixed by composing both filters together inside a single render() function that checks both state variables simultaneously.
GitHub Pages 404 — Deployment initially returned a 404 because the file wasn't named index.html. Renaming the entry point file resolved the issue immediately.


🌱 Future Features

 Interactive map view with pins per destination
 Images of what to expect
 Per-destination budget estimator
 Drag-and-drop trip planner for saved destinations
 Expanded destination library (50+ locations)
 Dark/light mode toggle
 Share itinerary via link
