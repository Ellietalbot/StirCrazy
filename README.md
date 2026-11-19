
# StirCrazy

**A full-stack cookbook website for organizing favorite recipes **

StirCrazy is a full-stack cookbook web application designed to help users discover, organize, save, and share their favorite recipes. Users can browse public recipes, build a personal cookbook called **MyCB**, add private notes, and create their own public or private recipes.

This repository contains the **frontend application** for StirCrazy.

## ✨ Features

The frontend is designed to provide a simple, cozy, and responsive experience for managing and discovering recipes.

### Planned Features

- **Home Page** – Explore featured recipes, navigate the application, and learn about StirCrazy.
- **Recipe Discovery** – Browse public recipes using searchable recipe cards.
- **Search & Filtering** – Search recipes and filter by categories, tags, and other criteria.
- **Recipe Details** – View recipe images, descriptions, ingredients, instructions, serving sizes, and cooking times.
- **User Authentication** – Register, log in, and log out of a personal account.
- **MyCB (My Cookbook)** – Save favorite recipes and organize a personal cookbook.
- **Personal Notes** – Add private notes to saved recipes.
- **Recipe Creation** – Create and manage personal recipes with public or private visibility.
- **Serving Size Conversion** – Adjust ingredient quantities based on the desired number of servings.
- **Responsive Design** – Access StirCrazy on desktop and mobile devices.

## 🎨 Design

StirCrazy uses a warm, cozy visual style inspired by the feeling of a personal cookbook.

### Color Palette

| Color | Hex Code |
|---|---|
| Brown | `#5D3A00` |
| Terracotta | `#AA422D` |
| Olive | `#9B8816` |
| Blush | `#EFB0A1` |
| Cream | `#EEE0CB` |

The interface prioritizes readability, intuitive navigation, recipe-focused layouts, and a consistent user experience.

## 🛠️ Technologies

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | Styling and responsive layouts |
| JavaScript | Frontend functionality and interactions |
| Svelte | Reusable components and reactive UI |
| Fetch API | Communication with the backend REST API |
| Git & GitHub | Version control and collaboration |
| Netlify | Frontend deployment |

## 🚀 Getting Started

Follow these instructions to run the frontend application locally.

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/)
- npm (included with Node.js)
- Git

### Installation

1. Clone the repository:

   ```bash
   git clone <frontend-repository-url>
   ```

2. Navigate into the project directory:

   ```bash
   cd stircrazy-frontend
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Start the development server:

   ```bash
   npm run dev
   ```

5. Open the local URL provided in your terminal to view the application.

## 🔌 Backend Connection

StirCrazy uses a separate backend repository built with Node.js, Express, and MongoDB.

The frontend communicates with the backend through RESTful API endpoints using the Fetch API.

### API Endpoints

The frontend will interact with endpoints such as:

| Method | Endpoint | Purpose |
|---|---|---|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Log in |
| POST | `/api/auth/logout` | Log out |
| GET | `/api/recipes` | Retrieve public recipes |
| GET | `/api/recipes/:id` | Retrieve a recipe |
| POST | `/api/recipes` | Create a recipe |
| PUT | `/api/recipes/:id` | Update a recipe |
| DELETE | `/api/recipes/:id` | Delete a recipe |
| GET | `/api/mycb` | Retrieve saved recipes |
| POST | `/api/mycb/:recipeId` | Save a recipe |
| DELETE | `/api/mycb/:recipeId` | Remove a saved recipe |
| PUT | `/api/mycb/:recipeId/notes` | Update a personal note |

The backend handles database operations, authentication, authorization, and data validation.

### Environment Variables

The frontend may require an environment variable to connect to the deployed or local backend.

For example, create a `.env` file:

```env
PUBLIC_API_URL=http://localhost:3000
```

Use the environment variable naming convention supported by the frontend build tool. For SvelteKit, public environment variables should use the appropriate `PUBLIC_` prefix.

**Note:** Never commit environment files containing private credentials or secrets.

## 📁 Project Structure

The frontend is organized to keep pages, reusable components, styling, and application logic maintainable.

Example structure (adapt as the project develops):

```text
stircrazy-frontend/
├── static/
│   └── images/
├── src/
│   ├── lib/
│   │   └── components/
│   ├── routes/
│   ├── css/
│   └── lib/
├── .env
├── .gitignore
├── package.json
└── README.md
```

The final structure may vary depending on the application's implementation and framework configuration.

## 👩‍🍳 Team

StirCrazy is developed collaboratively by four students for the Full Stack Foundations course.

| Team Member | Team Title |
|---|---|
| Matt | Grand Admiral |
| Emma | Master Chef |
| Ellie | Chief Technology Officer |
| Makayla | Team Principal |

All team members contribute to frontend development, backend development, testing, documentation, and project presentation.

## 🤝 Development Workflow

The team uses GitHub and Trello to coordinate development and manage project progress.

- **GitHub** – Source control, branches, commits, and collaboration.
- **Trello** – Task management, sprint planning, and progress tracking.
- **Microsoft Teams & Text Messaging** – Team communication.
- **Code Reviews** – Review changes before merging when practical.

### Contribution Guidelines

1. Create a feature branch for your changes.
2. Make focused changes with descriptive commit messages.
3. Test your changes locally.
4. Push your branch to GitHub.
5. Open a pull request for review when appropriate.
6. Merge approved changes into the main branch.

## 🧪 Testing

Frontend testing focuses on:

- Responsive layouts across desktop and mobile screens.
- Navigation and user interactions.
- Form validation and error handling.
- Authentication flows.
- Recipe browsing and search functionality.
- Recipe creation and editing.
- MyCB functionality and personal notes.
- Successful communication with backend API endpoints.

## 🚀 Deployment

The frontend application is planned to be deployed through **Netlify**.

The backend API is planned to be deployed separately through **Render**.

Both applications will communicate through the deployed API URL.

## 📅 Project Timeline

| Milestone | Deadline |
|---|---|
| Demo-ready application | December 10, 2026 |
| Final project submission | December 15, 2026 |

## 🔮 Future Improvements

Additional features may be implemented after the core application is complete:

- Recipe ratings and reviews.
- Comments and likes.
- Sharing recipes with friends.
- Following other users.
- Printing recipes.
- Connecting with other home cooks.

## 📚 Course Information

**Course:** Full Stack Foundations  
**Instructor:** Brother Thompson  
**Project:** StirCrazy  
**Final Deadline:** December 15, 2026

---

*Made with ❤️ and a little bit of kitchen chaos.*
