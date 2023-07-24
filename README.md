# Quote API

The Quote API is a simple RESTful API that allows you to fetch and create quotes. It provides endpoints to retrieve random quotes, fetch quotes by author, and add new quotes.

This is part of Codecademy's Full-Stack Engineer Career Path.

## Getting Started

To get started with the Quote API, follow these steps:

1. Clone the repository.
2. Install the dependencies by running `npm install`.
3. Start the server by running `node server.js`.
4. The server will start running on `http://localhost:4001`.

## Endpoints

The Quote API provides the following endpoints:

### GET /api/quotes/random

Returns a random quote from the collection of quotes.

Example response:

```json { "quote": "The greatest glory in living lies not in never falling, but in rising every time we fall.", "person": "Nelson Mandela" }```

### GET /api/quotes?person={author}

Returns quotes by the specified author.

Example request: `/api/quotes?person=Nelson Mandela`

Example response:

```json { "quotes": [ { "quote": "The greatest glory in living lies not in never falling, but in rising every time we fall.", "person": "Nelson Mandela" }, { "quote": "It always seems impossible until it's done.", "person": "Nelson Mandela" } ] }```

### POST /api/quotes?quote={quote}&person={author}

Adds a new quote to the collection.

Example request: `/api/quotes?quote=Be yourself; everyone else is already taken.&person=Oscar Wilde`

Example response:

```json { "quote": "Be yourself; everyone else is already taken.", "person": "Oscar Wilde" }```

## Dependencies

The Quote API uses the following dependencies:

- Express: A fast and minimalist web framework for Node.js.
- Morgan: A middleware for logging HTTP requests.
- Nodemon (devDependency): A utility that automatically restarts the server when changes are made during development.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).