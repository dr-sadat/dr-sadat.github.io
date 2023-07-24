# MongoDB_Resources

Download: https://github.com/dr-sadat/MongoDB_Resources 

Sample JSON files to use with MongoDB. These JSON files contain a varying number of documents, some less than ten, while others contain hundreds. 

You can import a JSON file to your MongoDB community server using the following command syntax: 

*mongoimport --collection=[Collection Name] --db=[Database Name] --type=json --jsonArray [FileName.json]*

Example: 

- macOS: `mongoimport --collection=Recipes --db=firstDatabase --type=json --jsonArray example.json`
- Windows: `mongoimport.exe --collection=Example --db=firstDatabase --type=json --jsonArray example.json`

Please note that the **--jsonArray** parameter in the above command needs to be included when the .JSON file contains multiple MongoDB documents within a single JSON array. If the file does not have such a structure, then remove the **--jsonArray** parameter from the command. 

For instance, the "movies.json" file does not need **--jsonArray** parameter and can be imported like below: 

- macOS: `mongoimport --collection=Recipes --db=firstDatabase --type=json movies.json`
- Windows: `mongoimport.exe --collection=Example --db=firstDatabase --type=json movies.json`

Therefore, check the .json file (by opening it in a text editor) before you import that document to identify whether it needs the --jsonArray parameter.
