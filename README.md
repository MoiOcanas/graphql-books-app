# GraphQL Books App

App for creating books with its author, name and genre. Also, gets all the authors with its books.

## Server
To start the server you need to go inside the server folder and run on your console:

```bash
npm install
nodemon app
```
## Client
Now, you've to go inside the client folder and run:

```bash
npm install
npm start
```

## Database
To use and configure your database. Go to MongoDB-Atlas and create or use your account. You need to create a new cluster and then just connect it with the project using the URL that MongoDB gives you.

Then go to server/app.js and paste the URL right here: 

```javascript
mongoose
 .connect(
  "YOUR MONGODB URL CONNECTION HERE",
  { useNewUrlParser: true, useUnifiedTopology: true }
 )
 .then(() => console.log("Connected to MongoDB Atlas"))
 .catch(err => console.log("Error: ", err.message));
```