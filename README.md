Student Help Desk
A complete, real-time Student Help Desk application built with HTML, CSS, and JavaScript, powered by Google Firebase for the backend. This project allows students to sign up, log in, submit support tickets, and engage in two-way communication with administrators.

(Note: You would need to take a screenshot of your live app and upload it to your repository to make this image link work)

Features
User Authentication: Secure sign-up and sign-in with Email/Password and Google Sign-In.

Ticket Submission: Students can create new support tickets with detailed descriptions of their issues.

Real-time Updates: The ticket list updates in real-time for both students and admins without needing to refresh the page.

Two-Way Communication: A full chat system within each ticket allows students and admins to communicate back and forth.

Admin Dashboard: Designated admins can view, manage, and reply to tickets from all users.

Status Tracking: Admins can mark tickets as "Open" or "Closed".

Responsive Design: The interface is optimized for both desktop and mobile devices.

Tech Stack
Frontend: HTML, Tailwind CSS, JavaScript (ESM)

Backend & Database: Google Firebase

Firestore: For the real-time NoSQL database.

Firebase Authentication: For managing user sign-up and login.

How to Set It Up
To run your own instance of this project, you will need to create a free Firebase project.

Create a Firebase Project: Go to the Firebase Console and create a new project.

Enable Authentication:

In the Firebase Console, go to Authentication -> Sign-in method.

Enable the Email/Password and Google providers.

Create Firestore Database:

Go to Firestore Database and create a new database.

Start in test mode for initial setup, but be sure to secure your rules for production.

Get Firebase Config:

In your project settings, find your web app's firebaseConfig object.

Update the Code:

Paste your unique firebaseConfig object into the <script> section of the index.html file.

Set Admin User:

Sign up for an account in your app that you will use for administration.

Find your User UID in the Firebase Authentication console.

Paste this UID into the adminUIDs array in the index.html file.

In Firestore, create a new collection called admins and add a document with your UID as the Document ID.

Deploy: Deploy the index.html file to a static hosting service like Netlify, Vercel, or GitHub Pages.
