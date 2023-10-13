# phoneBook_Backend
Steps for downloading on other workstations:

Run "npm init"
Run "npm install express"
Run "npm install --save-dev nodemon"


3.1: Phonebook backend step1
Implement a Node application that returns a hardcoded list of phonebook entries from the address http://localhost:3001/api/persons.

Data:

[
    { 
      "id": 1,
      "name": "Arto Hellas", 
      "number": "040-123456"
    },
    { 
      "id": 2,
      "name": "Ada Lovelace", 
      "number": "39-44-5323523"
    },
    { 
      "id": 3,
      "name": "Dan Abramov", 
      "number": "12-43-234345"
    },
    { 
      "id": 4,
      "name": "Mary Poppendieck", 
      "number": "39-23-6423122"
    }
]copy
Output in the browser after GET request:

JSON data of 4 people in browser from api/persons
Notice that the forward slash in the route api/persons is not a special character, and is just like any other character in the string.

The application must be started with the command npm start. //DONE

The application must also offer an npm run dev command that will run the application and restart the server whenever changes are made and saved to a file in the source code. //DONE


3.2: Phonebook backend step2
Implement a page at the address http://localhost:3001/info that looks roughly like this:

Screenshot for 3.2
The page has to show the time that the request was received and how many entries are in the phonebook at the time of processing the request.

There can only be one response.send() statement in an Express app route. Once you send a response to the client using response.send(), the request-response cycle is complete and no further response can be sent.

To include a line space in the output, use <br/> tag, or wrap the statements in <p> tags. //DONE