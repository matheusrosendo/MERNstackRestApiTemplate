# A MERN simple REST API template using MongoDb on Atlas free server and MongoDb extension on Visual Studio Code

Based on Mongodb tutorial [How to Use MERN Stack: A Complete Guide](https://www.mongodb.com/languages/mern-stack-tutorial).

![Licence](https://img.shields.io/github/license/matheusrosendo/TokenizationLabFixedSupply)
![main workflow](https://github.com/mongodb-developer/mongodb-express-rest-api-example/actions/workflows/main.yml/badge.svg)

## Requirements
* npm version ^16
* Visual Studio Code

## How To Run
0. Clone this repo

1. You can follow the [Getting Started with Atlas](https://docs.atlas.mongodb.com/getting-started/) guide, to learn how to create a free Atlas account, create your first cluster and get your Connection String to the database. 
Then, set the Atlas URI connection parameter in `server/.env` to your Connection String:
```
ATLAS_URI=mongodb+srv://<username>:<password>@sandbox.jadwj.mongodb.net/myFirstDatabase?retryWrites=true&w=majority
```

2. Start the Express server:
```
cd server
npm install
npm install -g nodemon
nodemon server
```
> you should see a "Successfully connected to MongoDB" message on terminal, let it running

3. Start the React app:
open another Terminal tab
```
cd client
npm install
npm start
```

4. Test App on localhost:3000
Create a Record
Edit that record


5. Install Visual Studio Code and MongoDB extension https://code.visualstudio.com/docs/azure/mongodb
* * Use the same connecting string contained in .env file to connect to Atlas MongoDb using the VS code MongoDb extension
* * Open MERNtutorial_employee_populate.mongodb and press 'Play' button

6. Check out new records inserted on both Atlas UI and localhost 
* Go to https://cloud.mongodb.com/
navigate to collections > MERNstackDB > employee and check new records just inserted
* Refresh your localhost:3000 on browser and check if the new records are there

7. You can also execute the other mongoDb files to get used to mongodb shell  sintax for insert, erase, update and delete data on mongodb:
* open server/db/MERNtutorial_* files and execute them



## Disclaimer

Use at your own risk; not a supported MongoDB product

