# FCC_TicketingApp

Next.js, Tailwind CSS, and MongoDB Project Tutorial – Ticketing App

https://www.freecodecamp.org/news/use-next-js-tailwind-css-and-mongodb-to-build-a-ticketing-application/

1. With Next.js, creating folders inside the main app folder automatically sets up a route with that structure.
   i.e., if we create a TicketApp folder, http://localhost:3000/TicketPage will be a valid URL for our application
   a) creating a folder with square brackets - i.e. [id] - will treat that folder name as a param.
   The param can then be accessed by the .jsx files inside that folder
   b) creating a folder with curved brackets - i.e. (components) - will make it so that the folder is not treated as a route.

2. Tailwind
   a) In the tailwind.config.js file, we can create css defaults for our application (need to dig into that).
   b) The globals.css file is set up with @base, @components and @utilities. Things can overwrite other properties depending on which one we're using.

3. Mongo and Mongoose
   a) Mongoose complements MongoDB by allowing the setting of Types.
   b) A Cluster is a group of Databases

4. Connecting to MongoDB
   a) After creating the DB (using the MongoDB web interface), go to Database > Connect > Drivers and copy the connection string into your application code
   b) Paste it inside .env.local, at the project's root folder
   c) Connect to it using mongoose.connect(process.env.<CONNECTION_STRING_VARIABLE>);
