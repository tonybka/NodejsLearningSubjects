# Environment variables in Nodejs
## Simple declaration in .bash_profile and usage
* Set value for SECRET_ACCESS_KEY
```
export SECRET_ACCESS_KEY=value
```
* Get value of SECRET_ACCESS_KEY from configuration file
```
var secretAccessKey = process.env.SECRET_ACCESS_KEY
```
Cause you might have more than one project on local development environment that also used same key name is SECRET_ACCESS_KEY => use dotenv
```
npm install -g dotenv
```

---
## Local project environment variables