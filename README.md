# ECommerce

## Description

Model of building the back-end for an e-commerce site. 


## Table of Contents

- [Installation](#installation)
- [DatabaseModels](#database models)
- [Usage](#usage)
- [License](#license)
- [Questions](#questions)

## Installation

Clone this project and run `npm install`. On MySQL CLI create the database with the following command in the root of the project. `source ./db/schema.sql`.Then seed the tables using `npm run seed`. Finally start the server running this command `nodemon server.js`.


## Database Models

* `Category`

  - `id`
    - *Integer*
    - *Not null*
    - *Primary key*
    - *Auto increment*

  - `category_name`
    - *String*
    - *Not null*

* `Product`
  - `id`
    - *Integer*
    - *Not null*
    - *Primary key*
    - *Auto increment*

  - `product_name`
    - *String*
    - *Not null*

  - `price`
    - *Decimal*
    - *Not null* 

  - `stock`
    - *Integer*
    - *Not null* 
    - *default 10*

  - `category_id`
    - *Integer*

* `Tag`
  - `id`
    - *Integer*
    - *Not null*
    - *Primary key*
    - *Auto increment*

  - `tag_name`
    - *String*
    - *Not null*

* `ProductTag` (Through Table)
  - `id`
    - *Integer*
    - *Not null*
    - *Primary key*
    - *Auto increment*

  - `product_id`
    - *Integer*

  - `tag_id`
    - *Integer*


## Usage

Use Insomnia to test RESTful API implementation with HTTP methods POST, GET, GET by id, PUT and DELETE by id.

## Video
https://watch.screencastify.com/v/QIlcO5ak9sQw6M0YQgES
## License

MIT License

Copyright (c) 2023 Rainy

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Questions

Check out my [GitHub](https://mzrainy.github.io/E-Commerce/)
Any questions regarding this project can be sent to IQ@gmail.com.