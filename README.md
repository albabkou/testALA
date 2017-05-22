*** Team ALA - Ahsan, Lisa, Aliaksei / 5.23.17 ***

# Book Bunch

## What is Book Bunch?

Contrary to popular belief, Millennials read more than older generations do—and more than the last generation did at the same age! An [article](https://www.theatlantic.com/technology/archive/2014/09/millennials-are-out-reading-older-generations/379934/) about the 2014 Pew Research Center report said that "Deeper connections with [books] are also often associated with key life moments such as having a child, seeking a job, being a student, and going through a situation in which research and data can help inform a decision." Soooo...basically all all of your 20's. Everything on the internet is interconnected. What better place to have a list of the books you've found on forbes, ESPN, instagram, in a youtube video, amazon etc. than Book Bunch. 

Book Bunch is a virtual bookshelf CRUD app where users can: 
- View books on a user profile archived in the database
- Add books to the (by searching the google books api)
- Edit books database, update the status of the book (read, reading, to-read), and add a review of the book.
- And delete books from the database

## Technologies To Be Used
- Express backend
- Postgres/Pg-Promise
- React
- Bcrypt/sessions (for user authentication)
- Git/Github.com
- CSS3
- Heroku web hosting

## Wireframes

#### Landing on home page

![img](path/name.png)


## Initial thoughts on database structure

Users.

| id | Username   | Email   | Password    | 
|--- |:----------:|:-------:| -----------:|
| 1  | 'username' | 'email' | 'password'  | 
| 2  | 'username' | 'email' | 'password'  | 
| 3  | 'username' | 'email' | 'password'  | 

Books.

| id | Title   | Author   | Genre  |   ISBN  |Description   | Rating | Image Url | Preview Link| 
|--- |:-------:|:--------:|:------:|:-------:|:------------:|:------:|:---------:| -----------:|
| 1  | 'title' | 'author' | 'genre'|  num    |'description' | num    | 'url'     |  'url'      |
| 2  | 'title' | 'author' | 'genre'|  num    |'description' | num    | 'url'     |  'url'      |
| 3  | 'title' | 'author' | 'genre'|  num    |'description' | num    | 'url'     |  'url'      |

Joined Table.

| id | User ref. id | Book ref id | Status   | Review     | 
|--- |-------------:|:-----------:| :-------:| ----------:|
| 1  |     1        |     1       |'Reading' | 'Loved it' | 
| 2  |     2        |     1       | 'Read'   | 'Hated it' |
| 3  |     1        |     2       | 'To-Read'| 'Loved it' |

## Advanced Features
- display books by status on user profile
- embedded/popup book preview
- Link to amazon to purchase books

## Links and Resources

- https://developers.google.com/books/
- http://developer.nytimes.com/books_api.json#/Documentation/GET/lists.%7Bformat%7D
- https://developers.google.com/books/docs/preview-wizard
- https://react-bootstrap.github.io/
- https://www.forbes.com/sites/neilhowe/2017/01/16/millennials-a-generation-of-page-turners/#255cd1fa1978

- https://git.generalassemb.ly/nyc-wdi-ada/ada-with-jointables