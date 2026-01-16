# 🏨 StayFlow – Full-Stack Hotel Booking Platform

**StayFlow** is a scalable, full-stack hotel booking application that enables users to discover, book, and manage hotel stays, while providing hotel owners with tools to list properties, manage rooms, and track bookings and revenue.  
The platform is built using modern web technologies with a strong focus on authentication, payments, and real-world production workflows.

---

## 🚀 Key Capabilities

### 👥 Guest Experience
- Search hotels by location and category
- View room details including amenities and pricing
- Book rooms with real-time availability checks
- Secure checkout using Stripe
- Receive booking confirmation emails
- Manage bookings through a user dashboard
- Authentication and session handling via Clerk

### 🏢 Hotel Owner Experience
- Register as a hotel owner
- Create, update, and remove room listings
- Upload and manage room images
- View booking history and revenue insights
- Access protected owner-only routes and dashboards

---

## 🔁 Application Workflow

- React frontend communicates with backend APIs using Axios
- Clerk manages authentication and session tokens
- Backend validates user identity via Clerk middleware
- MongoDB stores hotel, room, booking, and user data
- Cloudinary handles secure media uploads
- Stripe processes payments and payment confirmations
- Inngest manages asynchronous workflows
- Nodemailer sends transactional booking emails

---

## 🧰 Tech Stack

| Layer            | Technologies Used                         |
|------------------|-------------------------------------------|
| Frontend         | React (Vite), Tailwind CSS                |
| Backend          | Node.js, Express.js                       |
| Database         | MongoDB, Mongoose                         |
| Authentication  | Clerk                                     |
| Payments         | Stripe                                    |
| Email Services   | Nodemailer                                |
| Media Storage   | Cloudinary                                |
| Async Workflows | Inngest                                   |
| Deployment       | Vercel (Frontend), Render (Backend)       |

---

## 📁 Project Structure

```bash
StayFlow/
├── client/                  # Frontend (React + Vite)
│   ├── src/
│   │   ├── components/      # Reusable UI components
│   │   ├── pages/           # Application pages & routes
│   │   ├── context/         # Global state management
│   │   └── main.jsx         # App entry point
│   ├── public/
│   ├── .env.local
│   └── vite.config.js
│
├── server/                  # Backend (Express)
│   ├── configs/             # DB, Cloudinary, Email configs
│   ├── controllers/         # Business logic
│   ├── middleware/          # Auth & request handling
│   ├── models/              # Database schemas
│   ├── routes/              # API endpoints
│   ├── inngest/             # Background jobs & workflows
│   ├── .env
│   └── server.js            # Server entry point
