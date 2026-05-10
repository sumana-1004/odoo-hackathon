🌍 **Traveloop: Relational Itinerary & Budget Architect**
Traveloop is a comprehensive travel management "super-app" designed to streamline the planning process through a robust relational ecosystem.

🚀 **The Core Innovation (Relational Database)**

Unlike simple "list-based" travel apps, Traveloop uses a **PostgreSQL** relational schema to maintain strict data hierarchy:
- **Relational Integrity:** Trips act as the parent container for multiple **Stops** (Cities).
- **Nested Itineraries:** Each City Stop contains its own unique **Activities**, ensuring costs are tracked accurately by location.
- **Dynamic Budgeting:** Real-time cost aggregation through SQL queries, providing a visual breakdown of your travel spending.


Users can:
- create trips
- add cities and activities
- manage budgets
- make packing checklists
- share trip plans

## 🛠️ Quick Start
1. **Database:** Run `database/schema.sql` in the PostgreSQL terminal.
2. **Server:** `cd server && npm install && npm start`
3. **Client:** `cd client && npm install && npm run dev`

## Tech Stack

**Frontend:**
- React
- Vite (Fast HMR)
- Tailwind CSS (Responsive Design)
- Recharts (Dynamic Budget Pie Charts)

**Backend:**
- Node.js
- Express

**Database:**
- PostgreSQL (Chosen for relational data integrity)

**Features**
User authentication - JWT-based user authentication
Hierarchical Trip planning - Add multiple cities to a single trip and manage specific activities for each.
Multi-city itineraries
Intelligent Budget tracking - Automated cost tracking and category-wise spending charts.
Packing checklist - Trip-specific checklists to ensure travel readiness.
Collaboration - Generate unique read-only share links for friends and family.
Multi-city itineraries
Shareable trip links
Responsive UI


## FOLDER STRUCTURE 
client/    -> frontend
server/    -> backend API
database/  -> database related files
docs/      -> notes and planning
