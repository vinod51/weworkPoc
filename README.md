# weworkPoc

> api urls and request collection : import WeWork-MuleAPIs.postman_collection.json to postman 


Note: set below properties  while running the api. default values as below. change values as per the deployment


	mule.env   is set to dev , add environment propertiy to change or change in code for testing.



cartmanagement-exp-api 
	excample URL: 
	
	POST:   http://localhost:8083/api/cart/{customerId}
			body: 
			
			 [{
				
				"Spacetype": "dedicated",
				"capacity": 10,
				"Location": "Gaitheresburg",
				"MoveinDate": "2022-06-26",
				"MoveOutDate": "2022-06-30",
				"BillingFrq": "monthly",
				"Cost": "100",
				"Duration": 5
			  }]
			  
	GET:   http://localhost:8083/api/cart/{customerId}
	



properties:
	procapi.host=localhost     ProcessAPI HOST
	procapi.port=8082		   ProcessAPI PORT
	apiId=123




cartmanagement-proc-api

properties:
	sysapi.host=localhost
	sysapi.port=8081



cartmanagement-sys-api
	
	secure properties concept implimented but not applied yes. for demo purpose added to log to dispaly the decrypted value.
	
