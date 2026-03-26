# Travel Planner Project

A modern, responsive travel booking website inspired by platforms like MakeMyTrip, built to showcase comprehensive UI/UX design and frontend development skills using HTML, CSS, and Vanilla JavaScript.

## Description

The `Travel_Planner_Project` provides a complete conceptual frontend for a holiday booking application. It features an array of user flows including a dynamic Home Page with destination carousels, a comprehensive Holidays filtering and sorting system, and a detailed Package view with day-wise itineraries, image galleries, and reviews.

Key highlights include a "Trip Builder" wizard that guides users through creating custom itineraries (destination, hotel, transport, activities) and a multi-step booking/checkout flow featuring simulated payment integrations. It also provides a dashboard (`My Trips`) for users to view upcoming or past trips. While originally built as a frontend-only implementation, the repository is structured (with `backend/` and `frontend/` directories and Vercel configuration) to support future full-stack integration with MongoDB.

## How to Use and Run

### Run Locally
The application is primarily static HTML/CSS/JS, meaning it requires minimal setup:
1. **Clone the repository**:
   ```bash
   git clone https://github.com/spro047/Travel_Planner_Project.git
   cd Travel_Planner_Project/Travel_Planner
   ```
2. **Open the frontend**:
   Simply open `index.html` in any modern web browser to start exploring the site features. No local server is strictly required for the frontend UI.

### Deploying to Vercel
The repository includes a `vercel.json` configuration for easy cloud deployment:
1. Push your code to GitHub.
2. Log in to Vercel and import your repository.
3. Keep the "Framework Preset" as "Other".
4. **Important**: Set the "Root Directory" to `Travel_Planner` in the Vercel project settings.
5. If utilizing the `backend` folder, add `MONGO_URI` and `JWT_SECRET` in the Environment Variables section.
6. Click Deploy!

## Challenges Faced

Building a comprehensive travel platform mock-up presented several challenges:

1. **Complex UI State Management in Vanilla JS**: Simulating a multi-step "Trip Builder" and "Booking Flow" (handling cart details, generating summary prices dynamically, and checking validation across steps) required meticulous DOM manipulation and event listening without the aid of reactive frameworks like React or Vue.
2. **Extensive Filtering Logic**: Implementing the `holidays.html` filtering system—allowing concurrent sorting by Budget, Duration, Destination Type, and sorting by Popularity/Price—required robust JavaScript array filtering mechanics acting on simulated JSON data structures.
3. **Responsive Design Rigor**: Ensuring that complex layouts (like nested accordions for Day-wise itineraries, extensive table structures for booking reviews, and image gallery lightboxes) remained perfectly usable and visually distinct on mobile phones, tablets, and wide-screen desktops through CSS Grid and Flexbox media queries.
4. **Vercel Deployment Architecture**: Structuring a repository that houses both frontend static files and a potential backend API meant configuring `vercel.json` correctly and assigning the correct Root Directory so Vercel builds the entry points properly instead of treating the repo root as the project root.
