# **Social Media Mini App**

A lightweight social media platform where users can connect, share posts, and interact with others. Built using **Next.js** for a fast, scalable, and SEO-friendly experience.

---

## **Features**

1. **User Authentication**
   - Signup, login, and logout with NextAuth.js.
   - Secure session management.

2. **User Profiles**
   - Customize profile with a bio and profile picture.
   - Follow and unfollow users.

3. **Post Creation**
   - Create, edit, and delete posts (text and images).
   - Drag-and-drop image uploader.

4. **Interactive Feed**
   - View posts from followed users in a dynamic feed.
   - Infinite scrolling for seamless browsing.

5. **Likes & Comments**
   - Like posts and leave comments in real-time.

6. **Search & Explore**
   - Search for users or posts by keyword.
   - Discover trending posts on the explore page.

7. **Notifications**
   - Get notified about likes, comments, and followers.

---

## **Tech Stack**

### **Frontend**
- **Next.js**: Framework for SSR and API routes.
- **Tailwind CSS**: Modern, responsive UI styling.
- **React Query**: Efficient data fetching and caching.

### **Backend**
- **Node.js**: Server-side logic.
- **Next.js API routes**: For handling RESTful API endpoints.
- **Prisma ORM**: Database access and management.

### **Database**
- **PostgreSQL**: Relational database for user and post data.

### **Authentication**
- **NextAuth.js**: User authentication with Google or email/password.

### **Media Storage**
- **Cloudinary**: For image uploads and optimization.

### **Hosting**
- **Frontend:** Deployed on Vercel.
- **Backend/Database:** Hosted using Supabase or Railway.

---

## **Installation**

### Prerequisites:
- Node.js >= 16.x
- PostgreSQL instance
- Cloudinary account for media storage

### Steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/hyeonsooko/next-threads.git
   cd next-threads
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Configure environment variables:
   Create a `.env.local` file and add the following:
   ```
   DATABASE_URL=your_postgresql_url
   NEXTAUTH_SECRET=your_secret_key
   NEXTAUTH_URL=http://localhost:3000
   CLOUDINARY_URL=your_cloudinary_url
   ```

4. Initialize Prisma:
   ```bash
   npx prisma migrate dev
   ```

5. Run the app:
   ```bash
   npm run dev
   ```

6. Access the app at: `http://localhost:3000`

---

## **Deployment**

1. Deploy the app on **Vercel**:
   - Connect the GitHub repo to Vercel.
   - Add the `.env.local` variables to the Vercel dashboard.

2. Host the database using **Supabase** or **Railway**.

3. Use **Cloudinary** for production-ready media uploads.

---

## **Project Structure**
```
/pages
  /api        # Backend API routes
  /auth       # NextAuth.js configuration
  /profile    # User profile pages
  /feed       # Feed with posts
  /explore    # Explore trending posts

/components
  FeedItem.jsx
  ProfileCard.jsx
  CommentSection.jsx
  Navbar.jsx

/utils
  api.js      # API helpers
  auth.js     # Authentication utilities

/prisma
  schema.prisma  # Database schema
```

---

## **Future Improvements**
- Implement direct messaging between users.
- Add video support for posts.
- Improve notifications with a real-time system (e.g., WebSockets).
- Build a progressive web app (PWA) version for offline support.

---

## **Contributing**

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

---

## **License**

This project is licensed under the [MIT License](LICENSE).
