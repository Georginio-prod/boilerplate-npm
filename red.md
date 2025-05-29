## who to start a project 
for the first time, you run the command npm init -y for initialse the projet
and npm install express.
## add author
you can add 'author' to the package.json file to specify who is the author of the project.

## add description 
i add 'description' to describe what I'm doing in the project 

## add keywords
i add 'keywords' to specify the keywords that are related to the project.

## add license
i add 'license' to specify the license of the project.

## add version
i add 'version' to specify the version of the project.

## add dependencies
i add 'dependencies' to specify the dependencies of the project.

I change the version of "@freecodecamp/example": "1.1.0" on "@freecodecamp/example": "1.2.13"

add ~ to prefix the version of "@freecodecamp/example": "~1.2.13" or "^" to prefix the version of "@freecodecamp/example": "^1.2.13"

and I remove the "@freecodecamp/example": "^1.2.13"

## add file (myApp.js)
just a console.log("Hello World") in the file myApp.js

and secondly i create a route with app.get("/", (req, res) => {
  res.send("Hello Express!");
});

after this i declare a constant  let absolutePath = __dirname + "/views/index.html"; and send them with res.sendFile(absolutePath);

## dotenv
i add dotenv to the project and create a .env(secret) file with the variable PORT=3000. I use the condition to verif if req.json return me uppercase or not.

## get date
in this case a return the date with new Date().toString() and pass the route get("/now", (req, res) => {
  res.json({ time: new Date().toString() });
});

## get word 
for this case i create a route with app.get("/:word/echo", (req, res) => {
  const { word } = req.params;
  res.json({
    echo: word,
  });
});

## psot method
to declare bodyParser beacause he is previously installed on package.json

app.use(bodyParser.urlencoded({ extended: false }));
app.use(bodyParser.json()); 
In the next method return the name for the user 