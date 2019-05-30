# setting-mongo-db-environment
This course will teach you how to install and use mongo db database

# installing mongo database

Before you proceed with this tutorial, you will need to donwload and install Mongo db, in this course we will be using mongo db community edition

- MacOS https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/
- Linux https://docs.mongodb.com/manual/installation/
- Windows https://docs.mongodb.com/manual/tutorial/install-mongodb-on-windows/
- All downloads https://docs.mongodb.com/manual/installation/

On Windows make sure to add mongo db to the environmental variable path.

# working with mongo db

open a terminal and do the following;

Type mongo, this will get you into a mongo db shell. The mongo db shell allows you to interact with mongo db database and collections. You will notice that your prompt will change from the normal terminal prompt.You can exit mongo db shell by typing exit.

> Try to interact with the mongo db shell by following the tutorial on this link 
   - Mongodb shell basics https://docs.mongodb.com/manual/mongo/#working-with-the-mongo-shell
   - https://www.shellhacks.com/mongodb-create-database-and-user-mongo-shell/
   - https://www.freecodecamp.org/news/learn-mongodb-a4ce205e7739/
   - https://flaviocopes.com/mongodb/
   - https://docs.mongodb.com/manual/tutorial/backup-and-restore-tools/
   - https://docs.mongodb.com/manual/reference/program/mongodump/
   
  After interacting with the mongo database, create the following;
  
  - Create a database called entertainment
  - Create a collection called movies or music if you are not a fun of moviesin entertainment database
  - The schema for movies should be
  
  ```javascript
  
    movie: {
      title : 'movie title'
      releaseDate: 'date when the movie was released'
      producer : 'name of person who produced the movie'
      description: ' brief description of the movie'
 
    }
  ```
  - schema for music should be   
  ``` javascript
  
     song: {
       title: ' song title'
       releaseDate: 'when was the song produced'
       singer: 'who sang this song'
       description:' brief description of the song'
     }
  
  ```
  
  - Insert ten documents in the created collection (movies/music)
  - You can test you inserted document so that you familiarise with fetching documents in mongo db.
  

# Assignment

Hand in this aasignment by pushing this repository to github with your entertainment database which has either movies of music collection.

To hand in the database collection, do the following

- Open your terminal
- Navigate to the location of this repository
- Create a folder called database
- Navigate to database folder
- inside database folder do the following

```bash
  $ mongodump --db entertainment
  
```
This will create a folder in the database directory called dump which will have your entertainment mongo db database files.

- Push this repository to github and thats it
- The pushed repository should have a folder or folder url like 
       database/dump/entertainment/*.json or *.bson files
       
 
 Done







