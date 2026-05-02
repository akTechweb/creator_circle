🌐 Creator Circle – Creator Support Platform

Creator Circle is a full-stack crowdfunding platform that enables creators to receive direct support from their audience through secure online payments.

It was built to provide a simple and scalable way for independent creators to monetize their content and build a community.


📌 Key Features

- 🔐 Authentication using GitHub OAuth (NextAuth)
- 🧑 Creator profile customization (profile & cover image, payment credentials)
- ☕ Donation system (“Support a Creator”)
- 💳 Razorpay payment integration (order creation, verification, webhook handling)
- 📊 Creator dashboard with supporter leaderboard
- 🌐 Dynamic creator pages ("/username")
- ⚡ Server-side rendering using Next.js
- 📱 Fully responsive UI with Tailwind CSS
- 🔒 Secure API handling and session management

---

🛠️ Tech Stack

Frontend:

- Next.js 14
- React 18
- Tailwind CSS

Backend:

- Next.js API Routes
- Node.js

Database:

- MongoDB (Mongoose)

Authentication:

- NextAuth (GitHub OAuth)

Payments:

- Razorpay API

---

📂 Project Structure

creator-circle/
│── app/                # App Router (pages & layouts)
│── components/         # Reusable UI components
│── models/             # Mongoose schemas
│── db/                 # Database connection
│── app/api/            # Backend API routes
│── public/             # Static assets
│── utils/              # Helper functions

---

⚙️ Installation & Setup

1. Clone Repository

git clone https://github.com/your-username/creator-circle.git
cd creator-circle

2. Install Dependencies

npm install

3. Setup Environment Variables

Create ".env.local":

NEXT_PUBLIC_URL=http://localhost:3000
GITHUB_ID=your_github_client_id
GITHUB_SECRET=your_github_secret
MONGODB_URI=your_mongodb_connection
RAZORPAY_KEY_ID=your_key
RAZORPAY_SECRET=your_secret

4. Run the Project

npm run dev

---

💳 Payment Workflow

1. User initiates a donation
2. Backend creates Razorpay order
3. Razorpay checkout is triggered
4. Payment is processed
5. Signature verified on server
6. Payment stored in MongoDB
7. Dashboard updates with supporter data

---

🎯 Key Learnings

- Building scalable full-stack applications
- Payment gateway integration (Razorpay)
- Authentication and session management
- Production deployment and server configuration

---

🚀 Future Improvements

- Email notifications for payments
- Subscription-based memberships
- Advanced analytics dashboard
- Real-time updates




