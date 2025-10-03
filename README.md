# Library API Go Project
## Table of Contents
- [Project Name](#project-name)
- [About](#about)
- [Prerequisites](#prerequisites)
- [Features](#features)
- [Getting Started & Installation](#getting-started--installation)
- [Usage](#usage)
- [Learning Outcomes](#learning-outcomes)
- [Contributing](#contributing)
- [License](#license)
- [Credits & Acknowledgements](#credits--acknowledgements)
- [Contact](#contact)
## Project Name
Library API Go
## About
A RESTful API built in Go for managing a library catalog. This project implements a backend service to handle book operations such as adding, retrieving, updating, checking out, and returning books using HTTP endpoints with JSON data handling.
## Prerequisites
To run this project you need Go installed on your system. Additional libraries required:

-github.com/gin-gonic/gin for routing and handling HTTP requests

Install the dependency using:

`go get github.com/gin-gonic/gin`


## Features
This Library API Go includes these features:

-Retrieve all books via GET /books

-Retrieve a specific book by ID via GET /books/:id

-Create new books via POST /books

-Check out a book (decrease quantity) via PATCH /checkout?id=<id>

-Return a book (increase quantity) via PATCH /return?id=<id>

-JSON-based data handling for requests and responses

## Getting Started & Installation
Clone the repository to your local machine:


`git clone https://github.com/NickAlvarez20/libraryAPIGo.git`

Install dependencies:

`go get github.com/gin-gonic/gin`

## Usage
Run the Go script (main.go) from the command line:

`go run main.go`

The server will start on http://localhost:8080. Use tools like curl or Postman to interact with endpoints, e.g.:

curl http://localhost:8080/books to get all books

curl -X POST http://localhost:8080/books -H "Content-Type: application/json" -d '{"id":"4","title":"New Book","author":"Author Name","quantity":3}' to create a book

curl http://localhost:8080/checkout?id=1 to check out a book

## Learning Outcomes
This project helped me:

-Build a RESTful API using Go and the Gin framework

-Implement CRUD operations with query parameters and JSON handling

-Manage error handling and data validation in a Go-based API

-Understand Go's struct-based data modeling and HTTP routing

## Contributing
This is primarily a personal learning / portfolio repository, so formal contributions aren’t required. However, if you spot bugs, have project ideas, or want to add improvements, feel free to:
1. Fork the repo
2. Create a feature branch
3. Submit a pull request Please include clear explanations of your changes and test any new code.
## License
This repository is open and free for educational use.
*(If you decide on a specific license later, insert it here — e.g. MIT, Apache 2.0, etc.)*
## Credits & Acknowledgements
This project was created by NickAlvarez20 as part of my journey to learn Go programming. Check out my other repositories to see more of my work!
## Contact
You can find more of my work at [NickAlvarez20 on GitHub](https://github.com/NickAlvarez20).
