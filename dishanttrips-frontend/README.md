# DishantTrips frontend

Next.js interface for planning group trips, splitting expenses, and sharing travel memories.

## Development

```sh
npm ci
cp .env.example .env.local
npm run dev
```

Set `NEXT_PUBLIC_API_URL` in `.env.local` to your API origin. The default example uses `http://localhost:5000`.

Open http://localhost:3000. Start the backend separately using the instructions in the [project README](../README.md).

## Production check

```sh
npm run build
npm start
```
