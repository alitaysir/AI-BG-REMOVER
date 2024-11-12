# Background Removal SaaS Application

# Live Demo: [https://bg-removal-frontend-two.vercel.app/]

A full-stack MERN (MongoDB, Express, React, Node.js) SaaS application that allows users to remove the background from images. The app integrates **Clerk** for authentication and **Razorpay** for payment processing. Users receive **5 credits on login**, with **1 credit deducted per image edit**. Additional credits can be purchased if needed. The backend uses Clerk webhooks to manage user data effectively.

## Features

- **Background Removal**: Leverages the Clipdrop API to remove image backgrounds.
- **User Authentication**: Secured with Clerk authentication.
- **Credit System**: Users receive 5 free credits on login, with the ability to purchase additional credits.
- **Payment Integration**: Razorpay integration for easy payment processing.
- **Deployment**: Frontend and backend deployed on Vercel for seamless access.

## Tech Stack

- **Frontend**: React, deployed on Vercel
- **Backend**: Node.js, Express, MongoDB, deployed on Vercel
- **Payment Gateway**: Razorpay
- **Authentication**: Clerk, with webhooks for backend data synchronization
- **API**: Clipdrop for image background removal

## Prerequisites

- Node.js and npm installed
- Clerk account and API setup
- MongoDB URI and Clipdrop API Key
- Razorpay account (for payment integration)
- Optional: Stripe account setup

## Project Setup and Deployment

### Server Setup

1. **Open Project Folder**: Start by opening the project folder in VS Code or any preferred IDE.
2. **Setup Clipdrop API**: Obtain an API Key from [Clipdrop](https://clipdrop.co/apis).
3. **Setup MongoDB**: Create a MongoDB database and obtain your MongoURI from [MongoDB Atlas](https://www.mongodb.com/cloud/atlas/register).
4. **Razorpay Setup (Optional)**: Register and configure a Razorpay account [here](https://accounts.razorpay.com/auth).
5. **Stripe Setup (Optional)**: Register and configure a Stripe account [here](https://stripe.com/).
6. **Clerk Setup**: Register on [Clerk](https://clerk.com/) and set up authentication.
7. **Push to GitHub**: Push your project to a GitHub repository.
8. **Deploy Backend**: Deploy your backend on Vercel to obtain a backend URL. You can get started [here](https://vercel.com/).
9. **Setup Clerk Webhook**: Configure the Clerk webhook to handle user data and re-deploy your backend to Vercel. Find more info [here](https://dashboard.clerk.com/).

**Note**: Ensure the server is running before starting the client.

### Client Setup

1. **Open Folder in Terminal**: Navigate to the project directory and open the terminal.
2. **Install Dependencies**: Run the following command to install necessary dependencies:
     npm install
3. **Configure Environment Variables**: Add your backend URL and any other required environment variables in the .env file.
4. **Run Client**: Start the client with the command:
    npm run dev
5.**Deploy Client**: Deploy the client to Vercel by following the Vercel deployment process.
