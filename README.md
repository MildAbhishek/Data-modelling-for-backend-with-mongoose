# Simple express demo

> Express: fast, unopinionated, minimalist web framework for Node.js

This project shows a simple express server serving a single HTML page and using `express.static` to serve static files.

Check out the [express documentation](https://expressjs.com/) for more information.


# Mongoose is a JavaScript object-oriented programming library that creates a connection between MongoDB and the Node.js JavaScript runtime environment.

<!-- Official Documentation -->
# https://mongoosejs.com/

<!-- Data Modelling Diagram Tools -->
# https://www.datensen.com/data-modeling/moon-modeler-for-databases.html
# https://www.eraser.io/

# Here is the template level code for creating a model.

1. import mongoose from 'mongoose';

2. const userSchema = new mongoose.Schema({}, { timestamps: true });
<!--In first paramete type field i mandatory for every field,  second parameter { timestamps: true } gives two field by default ie, createdAt, updatedAt. -->

3. export const User = mongoose.model('User', userSchema);
<!-- 1st parameter is the name of table, by default mongoose convert it into plural starting with small letters. So, in DB `users` model will be created. Either we write User or users. Best practice is to write User instead users as we use to give reference in another model -->
