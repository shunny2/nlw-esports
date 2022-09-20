<p align="center">
<a href="#about-nlw-eSports">About NLW-eSports</a>
&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
<a href="#technologies">Technologies</a>
&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
<a href="#how-to-run">How to run</a>
&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
<a href="#status">Status</a>
</p>

</br>

![nlw](https://user-images.githubusercontent.com/72872854/191334230-85eb3cf3-221d-4c82-8f46-a0a60fba16e7.png)

## About NLW-eSports

NLW-eSports is a project that helps people find someone to play their favorite game.

## How to run

First, start by cloning the repository:
```shell
git clone https://github.com/shunny2/NLW-eSports
```

If you use docker, run the following command in the project root directory to run the frontend container.
```bash
docker-compose up -d
```

Interact with the docker container:
```bash
docker exec -it frontend /bin/bash
```

Finally, run the project with the command:
```bash
npm run dev
```

With the front end running, now let's start the backend. Access the backend folder with the command:
```shell
 cd backend
```

Inside the folder, run the command below to build the backend image.
```bash
docker-compose up -d --build
```

Okay. Your backend is already running.

Now we have to start the prism.

```bash
docker exec -it prisma-studio bash
```

Inside the prism container, run:
```bash
npx prisma generate
```

And finally, start prism studio:
```bash
npx prisma studio
```

Your page is available at the URL: [http://localhost:8000/](http://localhost:8000/)\
Your server is available at the URL: [http://localhost:3000/](http://localhost:3000/)\
Prism is available at the URL: [http://localhost:5555/](http://localhost:5555/)

## Technologies

- [ReactJS](https://reactjs.org/)
- [NodeJS](https://nodejs.org/)
- [Prisma](https://www.prisma.io/)
- [PostgreSQL](https://www.postgresql.org/)
- [Tailwindcss](https://tailwindcss.com/)

## Status

> Status: Developing.

<hr></hr>

<p align="center">Created by <a href="https://github.com/shunny2"><b>Alexander Davis</b><a/>.</p>