# 0x04. Files manager

![Statements](https://img.shields.io/badge/statements-90.69%25-brightgreen.svg?style=flat)
![Branches](https://img.shields.io/badge/branches-81.76%25-yellow.svg?style=flat)
![Functions](https://img.shields.io/badge/functions-88.52%25-yellow.svg?style=flat)
![Lines](https://img.shields.io/badge/lines-90.99%25-brightgreen.svg?style=flat)

Simple file management API that allows users to:

- Upload files
- Retrieve information about the files
- Download the files
- Share uploaded files with other users

## How to Run

Clone the repo

```
git clone https://github.com/nancyenos/alx-files_manager.git
```

Install required dependencies

```
cd alx-files_manager
npm install
```

Start worker

```
npm run start-worker
```

Start express server

```
npm run start-server
```

## Environment

Environment variables you can adjust when running the express server

- `PORT`: express server's port
- `DB_HOST`: mongodb's server host address
- `DB_PORT`: mongodb's port
- `DB_DATABASE`: database to use
- `FOLDER_PATH`: absolute path to folder to store files

## Documentation

The API's documentation is available at
[here]()

## Tests

Specify different `DB_DATABASE` and `FOLDER_PATH` environment when running test
to avoid data loss in main database and folder. Check out [test](tests/) folder
for unit tests.

- Run specific test

```
DB_DATABASE='test_database' FOLDER_PATH='/tmp/test_folder' npm test tests/testFile.js
```

- Run all tests

```
DB_DATABASE='test_database' FOLDER_PATH='/tmp/test_folder' npm run test-all
```


