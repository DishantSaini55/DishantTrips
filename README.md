# DishantTrips

Plan group trips, share expenses, and keep travel memories together.

Maintained by [Dishant Saini](https://github.com/DishantSaini55).

## Features

- Shared itineraries, trip roles, and group polls.
- Expense tracking and settlement suggestions.
- AI itinerary ideas and packing lists.
- Photo galleries, travelogues, and live meeting maps.
- Razorpay integration for premium upgrades.

## Stack

Next.js and React frontend, Express and Socket.IO backend, PostgreSQL with Prisma, Gemini, Cloudinary, Geoapify, and Razorpay.

## Local setup

Use Node.js 22.12 or later and a PostgreSQL database. Configure your own service credentials in local environment files.

Start the API:

```sh
cd dishanttrips-backend
npm install
cp .env.example .env
# Fill in your database URL and service credentials.
npx prisma generate
npx prisma db push
npm run dev
```

Start the frontend in another terminal:

```sh
cd dishanttrips-frontend
npm ci
cp .env.example .env.local
npm run dev
```

Open http://localhost:3000. The API runs at http://localhost:5000.

For deployment, set `NEXT_PUBLIC_API_URL` to your API URL and `FRONTEND_URL` to your frontend origin before building.

## Checks

```sh
cd dishanttrips-frontend
npm run build
```

## Project origin

Adapted from [Wandrly](https://github.com/SuryanshKS/Wandrly).
