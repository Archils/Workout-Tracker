# Workout Tracker

A fitness app for logging daily workouts and viewing progress over time, built with Express and MongoDB.

> The original Heroku deployment is no longer available because Heroku ended its free tier. Follow **Getting Started** to run it locally.

## Features

- Create a new workout or continue your last one
- Log multiple exercises per workout
- Track name, type, weight, sets, reps and duration for resistance exercises
- Track distance for cardio exercises
- Stats page with charts of workout duration and weight lifted over your last 7 workouts

## Built With

Node.js · Express.js · MongoDB · Mongoose · Morgan · Chart.js

## API Routes

| Method | Route | Description |
|---|---|---|
| GET | `/api/workouts` | All workouts, with total duration |
| GET | `/api/workouts/range` | Last 7 workouts, for the stats page |
| POST | `/api/workouts` | Create a workout |
| PUT | `/api/workouts/:id` | Add an exercise to a workout |

## Getting Started

**Prerequisites:** Node.js and MongoDB

```bash
git clone https://github.com/Archo2/Workout-Tracker.git
cd Workout-Tracker
npm install
npm run seed   # optional: add sample workouts
npm start
```

Then open http://localhost:3000. The app connects to `mongodb://localhost/workout` unless you set a `MONGODB_URI` environment variable.

## Author

**Archils Oburu**
- GitHub: [@Archo2](https://github.com/Archo2)
- Email: oburuarchils@gmail.com
