# 🌐 My Awesome Blog Platform

![Project Banner](https://your-image-link-here.com/banner.png)

> A modern, fully-featured blog platform using **Next.js** for the frontend and **Strapi 5** as the headless CMS backend, designed to deliver an exceptional user experience and flexible content management.

---

## 📝 Table of Contents

1. [About the Project](#about-the-project)
2. [Features](#features)
3. [Demo](#demo)
4. [Tech Stack](#tech-stack)
5. [Installation](#installation)
6. [Usage](#usage)
7. [API Documentation](#api-documentation)
8. [Project Structure](#project-structure)
9. [Contributing](#contributing)
10. [License](#license)

---

## 🌟 About the Project

Welcome to **My Awesome Blog Platform** – a versatile and customizable blogging platform created with **Next.js** and **Strapi**. This project offers a powerful and user-friendly setup, allowing for effortless content management and a polished, responsive front-end. Built with a focus on scalability and performance, it is perfect for bloggers, writers, and content creators.

![Blog Preview](https://your-image-link-here.com/preview.png)

---

## 🚀 Features

- **Modern UI/UX**: Sleek, responsive design powered by Next.js and Tailwind CSS.
- **SEO-Friendly**: Optimized for search engines to improve visibility.
- **Dynamic Content Management**: Utilize Strapi's CMS capabilities for effortless content creation.
- **Authentication & Authorization**: Secure user login and role-based permissions.
- **Image Optimization**: On-the-fly image optimization for fast loading.
- **Comments and Likes**: User interactions to enhance engagement.
- **Search and Filter**: Find specific articles quickly and easily.
- **Pagination**: Efficient loading for articles across pages.
- **Markdown Support**: Write content using Markdown for flexibility.
- **Social Sharing**: Share posts on major social platforms.

---

## 🎥 Demo

> **[Live Demo Here!](https://your-live-demo-link.com)**

![Live Demo Screenshot](https://your-image-link-here.com/demo.png)

---

## 🛠️ Tech Stack

| Frontend | Backend  | Database   | Authentication | API     |
| -------- | -------- | ---------- | -------------- | ------- |
| Next.js  | Strapi 5 | MongoDB    | JWT            | REST    |
| Tailwind | Node.js  | PostgreSQL | OAuth          | GraphQL |

---

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

---

## 🚀 After Installation

Once you’ve completed the installation steps, here’s how to set up the project and customize it further:

### 1. Initialize Strapi (Backend)

- After running `npm run develop` in the backend folder, open your browser and go to:
  ```
  http://localhost:1337/admin
  ```
- Create an admin account on the initial setup screen.
- Set up your content types for blog posts, categories, tags, and users as needed.

### 2. Configure Permissions

- In Strapi, go to **Settings** > **Roles** > **Public**.
- Enable read permissions for `Posts` and any other content types you want to be publicly accessible.
- Save your changes to make sure the public can view the content on the frontend.

### 3. Set Up Frontend API Connections

- Your frontend (Next.js) should be configured to connect to the Strapi backend using the environment variable `NEXT_PUBLIC_API_URL`.
- Double-check that this variable is correctly set in `frontend/.env.local`:
  ```plaintext
  NEXT_PUBLIC_API_URL=http://localhost:1337
  ```
- This setup allows Next.js to dynamically fetch content from Strapi.

### 4. Customize Site Metadata

- Edit `frontend/next.config.js` to adjust site-level metadata, such as title and description:
  ```javascript
  module.exports = {
    reactStrictMode: true,
    env: {
      SITE_TITLE: "My Awesome Blog Platform",
      SITE_DESCRIPTION: "A modern blog platform powered by Next.js and Strapi",
    },
  };
  ```

### 5. Start Developing 🚧

- Run both the backend and frontend in development mode:

  ```bash
  # Backend
  cd backend
  npm run develop

  # Frontend
  cd ../frontend
  npm run dev
  ```

- Open your browser and navigate to `http://localhost:3000` to see your blog in action!

### 6. Deployment (Optional)

- When you’re ready to go live, refer to the [Next.js deployment documentation](https://nextjs.org/docs/deployment) and [Strapi deployment guides](https://strapi.io/documentation/developer-docs/latest/setup-deployment-guides/deployment.html) for a seamless launch.

---

> 💡 **Tip**: Use [Strapi Plugins](https://strapi.io/documentation/developer-docs/latest/plugins/plugins-intro.html) to extend your blog’s capabilities with features like email notifications, media library optimization, and more!

# 2. Install dependencies

```
# Frontend
cd frontend
npm install

# Backend
cd ../backend
npm install
```

# Backend

cd ../backend
npm install
Environment Variables
Create .env files for both frontend and backend with necessary variables:

Frontend (frontend/.env.local)

plaintext
Copy code
NEXT_PUBLIC_API_URL=http://localhost:1337
Backend (backend/.env)

plaintext
Copy code
DATABASE_URL=your-database-url
JWT_SECRET=your-secret-key
Run the project

bash
Copy code

# Backend (Strapi)

```
cd backend
npm run develop
```

# Frontend (Next.js)

cd frontend
npm run dev
📖 Usage

1. Content Management (Strapi)
   Access the Strapi CMS at http://localhost:1337/admin.
   Create and manage blog posts, categories, and media files.
2. Frontend (Next.js)
   Visit http://localhost:3000 to view the blog.
   Users can browse posts, interact with content, and share articles.
   📚 API Documentation
   Authentication

POST /auth/local - Login
POST /auth/local/register - Register
Blog Posts

GET /posts - Fetch all posts
GET /posts/:id - Fetch a specific post
POST /posts - Create a new post (admin only)
Comments

POST /comments - Add a comment
GET /comments/:postId - Get comments for a post
More endpoints and details can be found in the API docs.

## 🗂️ Project Structure

```
my-awesome-blog/
├── frontend/       # Next.js frontend
│   ├── components/ # Reusable components
│   ├── pages/      # Next.js pages
│   └── styles/     # Global styles and Tailwind CSS
└── backend/        # Strapi CMS backend
    ├── api/        # API endpoints and content types
    └── config/     # Strapi configurations

```

# 🤝 Contributing

We welcome contributions to make this project better! If you'd like to contribute, please:

Fork the repository.
Create a new branch (git checkout -b feature/new-feature).
Commit changes (git commit -m 'Add new feature').
Push the branch (git push origin feature/new-feature).
Create a Pull Request.
📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

📬 Contact
Feel free to reach out with any questions or suggestions!

📧 mahfujurrahman06627@gmail.com

Made with ❤️ by Mahfujur Rahman
