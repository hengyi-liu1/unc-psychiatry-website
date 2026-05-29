# Starting the Application

In its current state, the application is not deployed to a server and must be run locally at `http://localhost:4200`.

## Prerequisites

Install the following before starting the application:

- Angular CLI
- Node.js v18
- MongoDB Community Server v7.0

## Email Invitation Feature Setup

To use the email invitation feature, create a .env file inside the api folder and add the following environment variables using your Gmail address and a Gmail App Password (not your regular password):

```env
EMAIL_USERNAME=your-email@gmail.com
EMAIL_PASSWORD=your-app-password
```

## Install Frontend Dependencies

Open a terminal and run:

```bash
cd my-app
npm install
```

## Install Backend Dependencies

Open another terminal and run:

```bash
cd api
npm install
```

## Start the Backend Server

Run the following command:

```bash
cd api
npx tsx src/app.ts
```

## Start the Frontend Server

In a separate terminal, run:

```bash
cd my-app
ng serve
```

## Start MongoDB

Make sure your MongoDB server is running:

```bash
brew services start mongodb-community@7.0
```

## Open the Application

Once all services are running, open your browser and navigate to:

```bash
http://localhost:4200
```

## Stop MongoDB

To stop the MongoDB server, run:

```bash
brew services stop mongodb-community@7.0
```
