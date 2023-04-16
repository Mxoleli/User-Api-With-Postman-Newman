# User-Api-With-Postman-Newman
You will need to install the below packages in order to run this framework locally.
  1. Newman package -  npm install -g newman
  2. Newman Report -  npm install -g newman-reporter-htmlextra

Newman commands to run the tests

| Operations                                    | Commands                                                                    | 
| --------------------------------------------- |:---------------------------------------------------------------------------:| 
| Simple collection                             | run	newman run UserCollection.json                                          | 
| Run a collection with environment details     | newman run UserCollection.json -e TestEnv.json                              |  
| Run a collection with an external data source | newman run UserCollection.json -e TestEnv.json -d UserData.csv              |
| Generate Junit report                         | newman run UserCollection.json -e TestEnv.json -d UserData.csv -r htmlextra |
