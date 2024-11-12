# Twitter Clone

A Twitter-like social media application built with Next.js, aiming to replicate core Twitter functionalities such as user profiles, posts (tweets), likes, and retweets. This project was created for educational purposes to practice Next.js and full-stack development skills.

## Features

- **User Authentication**: Sign up and log in to create an account.
- **Profile Management**: Users can edit their profile information.
- **Tweets**: Post, delete, like, and retweet tweets.
- **Feed**: Displays a feed of all posts and updates in real time.
- **Responsive Design**: Optimized for both desktop and mobile devices.

## Tech Stack

- **Frontend**: Next.js, Tailwind CSS
- **Backend**: API routes in Next.js
- **Database**: (Choose from PostgreSQL, MongoDB, or Firebase based on your setup)
- **Authentication**: NextAuth.js or Firebase Authentication
- **State Management**: Context API / Zustand / Recoil (choose one as per your setup)

## Getting Started

### Prerequisites

- Node.js (>= 16.x.x)
- npm or yarn

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/twitter-clone.git
    cd twitter-clone
    ```

2. Install dependencies:

    ```bash
    npm install
    # or
    yarn install
    ```

3. Set up environment variables:

   Create a `.env.local` file and add the following:

    ```plaintext
    DATABASE_URL=your_database_url
    NEXTAUTH_SECRET=your_secret
    NEXTAUTH_URL=http://localhost:3000
    ```

4. Run the development server:

    ```bash
    npm run dev
    # or
    yarn dev
    ```

    Open [http://localhost:3000](http://localhost:3000) in your browser to view the application.

### Database Setup

- If using **PostgreSQL**: Use `prisma` or another ORM to handle migrations and data seeding.
- If using **MongoDB**: Connect via `mongoose` or the native MongoDB driver.

### Authentication Configuration

- Configure NextAuth.js for user authentication. Update providers (such as Google, GitHub) in the `[...]auth.ts` file in `/pages/api/auth`.

## Scripts

- `dev`: Runs the app in development mode.
- `build`: Builds the app for production.
- `start`: Starts the app in production mode.

## Folder Structure

```plaintext
/twitter-clone
├── components        # Reusable UI components
├── pages             # Next.js pages
├── public            # Static files
├── styles            # Global and component-specific styles
├── utils             # Utility functions
├── .env.local        # Environment variables
└── README.md
```

## Future Improvements

- Add direct messaging.
- Implement hashtags and search functionality.
- Add notifications for new followers, likes, and retweets.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or suggestions.

## License

This project is open-source and available under the MIT License.

