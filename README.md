<img alt="GoStack Banner" src="./banner.png" />

<h3 align="center">
  Challenge 04: React-Native Concepts
</h3>

<p align="center">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/thadeucity/go-stack_challenge_05?color=%2304D361">

  <a href="https://github.com/thadeucity">
    <img alt="Made by Victor Alvarenga" src="https://img.shields.io/badge/made%20by-Victor Alvarenga-%2304D361">
  </a>

  <img alt="License" src="https://img.shields.io/badge/license-MIT-%2304D361">

</p>

<p align="center">
  <a href="#rocket-about-the-challenge">About the Challenge</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-license">License</a>
</p>

## :rocket: About the Challenge

This was the fifth challenge for the Go-Stack Bootcamp. It involved the creation of a Node.js API to handle cash flow in a single account. The user is able to post an <b>Income</b> or <b>Outcome</b> of money with a `POST` route and get the ballance in the account with all the transactions with a `GET` route.

Click [HERE](https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-fundamentos-nodejs) to see the full challenge description (PT-BR).

### Technologies
This project was developed with [Node.js](https://nodejs.org/en/)

### API Routes

- `POST /transactions` : The route should receive `title`, `value` and `type` inside the request.body, the type should be `income` or `outcome` and the result should be stored in an object following this template:
```js
{
  "id": "uuid",
  "title": "Salary",
  "value": 3000,
  "type": "income"
}
```

- `GET /transactions `: This route should list all the transactions the user registered until now, and should also give the `Sum` for the Outcome, the Income and the Account total Balance. Returning an abject following the template listed below:
```js
{
  "transactions": [
    {
      "id": "uuid",
      "title": "Salary",
      "value": 4000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Fiver Freelance",
      "value": 2000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Credit Card",
      "value": 4000,
      "type": "outcome"
    },
    {
      "id": "uuid",
      "title": "Gaming Chair",
      "value": 1200,
      "type": "outcome"
    }
  ],
  "balance": {
    "income": 6000,
    "outcome": 5200,
    "total": 800
  }
}
```

### Tests

To pass the challenge the project:

- **`should be able to create a new transaction`**

- **`should be able to list the transactions`**

- **`should not be able to create outcome transaction without a valid balance`**

## :memo: License

This project is under the MIT license. See the [LICENSE](LICENSE.md) for details.

---

Made with ♥ by Victor Alvarenga :wave: [Get in touch!](https://www.linkedin.com/in/victoralvarenga/)
