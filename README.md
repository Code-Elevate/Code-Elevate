# CodeElevate - Coding Contest Platform

CodeElevate is a coding contest platform where you can create and participate in coding contests. You can create contests, add problems, and participate in contests. You can also view the leaderboard of the contests.

## Hosted Links

| Hosting       | Link                                                                              |
| ------------- | --------------------------------------------------------------------------------- |
| Frontend      | [code-elevate.gopalsaraf.com](https://code-elevate.gopalsaraf.com/)               |
| Backend       | [code-elevate.gopalsaraf.com/api](https://code-elevate.gopalsaraf.com/api/)       |
| Engine        | [code-elevate.gopalsaraf.com/engine](https://code-elevate.gopalsaraf.com/engine/) |
| Documentation | [code-elevate.gopalsaraf.com/docs](https://code-elevate.gopalsaraf.com/docs/)     |

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

- Git
- Docker
- Docker Compose
- Node.js

**Note**: For detailed instructions on how to install these dependencies, [click here](EC2.md).

### After system dependencies are installed, clone this repository:

```sh
git clone --recurse-submodules https://github.com/Code-Elevate/Code-Elevate
```

### Navigate to the repository

```sh
cd Code-Elevate
```

### Edit the .env file to configure the backend

#### Rename the `.env.example` file to `.env`

```sh
mv .env.example .env
```

#### Edit the `.env` file

```sh
nano .env
```

While editing the `.env` file, make sure to fill in the REQUIRED fields. Without these fields, the backend will not work.

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
