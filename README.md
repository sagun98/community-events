## Community Events (Cheat sheet):

### MLAB setup (Remote mongodb Database)  
- #### Create account in `mlab.com` and new user.  
    
  
### Drywall(aqua-master) setup for login and authentication:  
- #### Clone or Download the drywall(aqua-master) on the project folder and configure `config.js`
- #### Set the mongodb URI, emails and passwords:
```bash
    mongodb: {
            uri: {
                $filter: 'env',
                production: process.env.MONGODB_URI,
                test: 'mongodb://sagun98:sagunis1@ds145158.mlab.com:45158/comeventsapp',
                $default: 'mongodb://sagun98:sagunis1@ds145158.mlab.com:45158/comeventsapp'
            }
        }
``` 
- ### Before hitting npm install, first change the dependency of bcrypt to bcryptjs and update the version of it.

commit update