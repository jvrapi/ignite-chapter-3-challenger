![Ignite Logo](https://repository-images.githubusercontent.com/341683746/42e1ab80-77af-11eb-9e07-47f9e46b3e6e)

<p align="center">
  <a href="#-about">About</a>
  &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-challenges">Challenges</a>
  &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-configurations">Configurations</a>
  &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-license">License</a>

</p>


## 🚀 About 
This is main challenge of chapter 3. The objective is use the different's ways to work with [typeorm](https://typeorm.io/).

## 🔥 Challenges
In [users repository](./src/modules/users/repositories/implementations/UsersRepository.ts), the methods should:

- [x] Using ORM, the method `findUserWithGamesById` should be able to receive an ID and return the user data, including all games they have.
- [x] Using Raw SQL, the method `findAllUsersOrderedByFirstName`should be able to list all users,ordering by first name in ascending away
- [x] Using Raw SQL, the method `findUserByFullName` should be able to receive the first and last name and return the users with the same first and last name, ignoring the uppercase arguments


In [games repository](./src/modules/games/repositories/implementations/GamesRepository.ts), the methods should:

- [x] Using the Query Builder, the `findByTitleContaining` method should be able to take an argument and return all games that contain the argument in the title.
- [x] Using the Raw SQL, the `countAllGames` method should be able to count all games registered.
- [X] Using Query Build, the `findUsersByGameId` method should be able to take a game id and return all users who own the game.

## ⚙️ Configurations
To run this repository, it's necessary that  you have the Postgres in your machine. If you use `docker`, you can run this command:

```bash
docker run --name ignite-challenge-database-queries -e POSTGRES_DB=queries_challenge -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres
```
This command will create a Postgres container with database `queries_challenge`.

With you already have the Postgres in you machine, you need to create a database with name `queries_challenge` so that the tests can work.

To run tests, you need to execute the command: 

```bash
  npm run test
```
Or using yarn:

```bash
yarn test
```

## 📝 License
You can should the license [here](./LICENSE)

---

<div align="center">

Feito com ❤ por [João Vitor Santos](https://github.com/jvrapi) 👋 Entre em contato!

[![Linkedin Badge](https://img.shields.io/badge/-João%20Vitor-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/joaovitorssdelima/)](https://www.linkedin.com/in/joaovitorssdelima/)
[![Gmail Badge](https://img.shields.io/badge/-Gmail-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:joaooviitoorr@gmail.com)](mailto:joaooviitoorr@gmail.com)
[![Hotmail Badge](https://img.shields.io/badge/-Hotmail-0078d4?style=flat-square&logo=microsoft-outlook&logoColor=white&link=mailto:joaooviitorr@hotmail.com)](mailto:joaooviitorr@hotmail.com)

</div>


