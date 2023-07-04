# MongoDB_Resources

Sample JSON files to use with MongoDB. These JSON files contain a varying number of documents, some less than ten, while others contain hundreds. 

You can import a JSON file to your MongoDB community server using the following command syntax: 

*mongoimport --collection=[Collection Name] --db=[Database Name] --type=json --jsonArray [FileName.json]*

Example: 

- macOS: `mongoimport --collection=Recipes --db=firstDatabase --type=json --jsonArray example.json`
- Windows: `mongoimport.exe --collection=Example --db=firstDatabase --type=json --jsonArray example.json`
