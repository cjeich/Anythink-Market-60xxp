# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

0. Download the repository and cd into the directory
```
$ git clone  git clone git@github.com:<github-username>/Anythink-Market-60xxp.git
$ cd Anythink-Market-60xxp
```

### 1. Start Docker
```bash
$ docker compose up
```

### 2. Navigate to backend API
http://localhost:3000/api/ping

### 3. Run Rails Migrations
Click run migrations in UI

or

start a shell in the docker image:

```bash
$ docker exec -it anythink-backend bash
$ cd backend
$ rails db:migrate

# check all migrations have run
$ rails db:migrate:status
```

### 4. Check that the front end is working

Go to: http://localhost:3001/register

You should see the site login page!

### 5. Create a user and log in.
