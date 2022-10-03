# (Beta) Postman script for API
THIS IS TO BE USED FOR EVALUATION PURPOSE ONLY. WE ARE NOT HOLDING ANY ACCOUNTABILITY AND RESPONSIBILITY AGAINST ANY CASES OF OUTCOMES BY UTILIZING THE SCRIPTS SHOWN IN THIS REPOSITORY 

Postman collections for simple API call to Equinix Fabric product.

[Equinix Fabric Portal](https://fabric.equinix.com/)

## Contents
- Token_generator
- VC_lookup
- NE_lookup
- creation_NEtoPort_VC
- creation_NEtoAzure_ExR_VC

## Prerequisites
1. You need [Postman](https://www.postman.com/downloads/) in your machine to call an API with the script in this repo.
2. You need to have a valid account of [Equinix Fabric Portal](https://fabric.equinix.com/). Please reach out to your CSM if you don't have one.
3. You need to have a valid account of [Equinix Developer Platform](https://developer.equinix.com/). Please reach out to your CSM if you don't have one.
4. You need to generate **client_id** and **client_secret**. please follow the [guide](https://developer.equinix.com/docs?page=/dev-docs/fabric/overview).
5. You need [Github](https://github.com/) account.

## How to setup
1. Launch [Postman](https://www.postman.com/)
2. Follow the steps per [guide](https://learning.postman.com/docs/getting-started/importing-and-exporting-data/#importing-from-github-repositories) to import the data into postman.
3. Fill up variables with your own.
   - Click **Environment quick look** at the top right corner.
     - <sub>Postman</sub>
     - ![env quicklook](https://user-images.githubusercontent.com/109955201/193489769-ee15fbdf-7e55-4c93-9621-3630e2fbcde8.png)
   - **client_id** and **client_secret** in current value field should be what you see on [Equinix Developer Platform](https://developer.equinix.com/).
     - <sub>Equinix developer platform</sub>
     - <img width="656" alt="userinfo" src="https://user-images.githubusercontent.com/109955201/193498978-87897281-25d6-4c3f-bd26-3532dccc2658.png">
     - <sub>Postman</sub>
     - <img width="703" alt="userinfo2" src="https://user-images.githubusercontent.com/109955201/193501814-47b94912-ef0b-4b5c-9e23-b5cbbf3d8700.png">
   - fill up **vc_uuid**, **ned_uuid**, and other parameters as well for your call.

---
## Use case

### VC lookup

1. Generate **access_token** by calling API with "Token_generator" collection.
2. Make a call with "VC_lookup" collection.
   - <sub>response successful</sub>
   - ![response](https://user-images.githubusercontent.com/109955201/193509583-0e1c055c-2b3e-4141-88d5-4ac91b88fdaf.png)
