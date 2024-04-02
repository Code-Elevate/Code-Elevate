# CodeElevate - Coding Contest Platform

CodeElevate is a coding contest platform where you can create and participate in coding contests. You can create contests, add problems, and participate in contests. You can also view the leaderboard of the contests.

## Hosted Version

A hosted version of this platform is available at [CodeElevate](https://code-elevate.gopalsaraf.com/).

### Frontend - [CodeElevate Frontend](https://code-elevate.gopalsaraf.com/)

### Backend - [CodeElevate Backend](https://code-elevate.gopalsaraf.com/api/)

### Engine - [CodeElevate Engine](https://code-elevate.gopalsaraf.com/engine/)

### Documentation - [CodeElevate Documentation](https://code-elevate.gopalsaraf.com/docs/)

## Features

- Create contests
- Add problems to contests
- Participate in contests
- View leaderboard of contests
- Live collabraion with other team members
- Chat with other team members

## Deployment

This system is designed to be deployed as a Docker container. It is recommended to use the provided `compose.yml` file to deploy the system.

### Host System Package Dependencies

- Docker
- Docker Compose
- Node.js

### After system dependencies are installed, clone this repository:

```sh
git clone --recurse-submodules https://github.com/Code-Elevate/Code-Elevate
```

### Navigate to the repository

```sh
cd Code-Elevate
```

### Edit the .env file to configure the backend

#### Navigate to the backend directory

```sh
cd Backend
```

#### Rename the `.env.example` file to `.env`

```sh
mv .env.example .env
```

#### Edit the `.env` file

```sh
nano .env
```

While editing the `.env` file, make sure to fill in the REQUIRED fields. Without these fields, the backend will not work.

### Navigate back to the root directory

```sh
cd ..
```

### Start the system

```sh
docker-compose up -d
```

## Additional Commands

### To view logs

```sh
docker-compose logs
```

### To stop the system

```sh
docker-compose down
```

### To terminate the system

```sh
docker-compose stop
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
