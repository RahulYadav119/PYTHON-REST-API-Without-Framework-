# Building REST apis with Nodejs without using any framework or external library

The final.py is simple HTTP server which can host the following api's :

VIEW : Uses VIEW Method to show the Value for a given Key from the db.json file.

LIST : Uses GET Method to show all the Values from the db.json file.		

CREATE : Uses POST Method to Create a new member for the db.json file.

UPDATE : Uses PUT Method to update an Existing member of the db.json file.

DELETE : Uses DELETE Method to delete an Existing member from the db.json file.
		

Usage of VIEW:  `$curl -X VIEW --data "<Key>" 127.0.0.1:8080`

Usage of LIST: `$curl -X GET 127.0.0.1:8080`

Usage of CREATE:  `$curl -X POST --data "<New_Value>" 127.0.0.1:8080`

Usage of UPDATE: `$curl -X PUT --data "<KEY>.<UPDATED_VALUE>" 127.0.0.1:8080`

Usage of DELETE: `$curl -X DELETE --data "<KEY>" 127.0.0.1:8080`
	
	

## For Instance,

	$curl -X VIEW --data "1" 127.0.0.1:8080
	
	$curl -X GET 127.0.0.1:8080
	
	$curl -X POST --data "NEW_DATA" 127.0.0.1:8080
	
	$curl -X PUT --data "5.UpdatedData" 127.0.0.1:8080
	
	$curl -X DELETE --data "5" 127.0.0.1:8080
