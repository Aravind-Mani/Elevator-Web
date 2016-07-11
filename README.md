# Elevator-Web
The Elevator Web Project

The web interface serves as the monitor to remote security team to know the status of the two elevators. The service exposed URL are

GET http://elevator-env.ap-southeast-2.elasticbeanstalk.com/webapi/elevators (returns the details of the elevator either in JSON or XML format)

POST http://elevator-env.ap-southeast-2.elasticbeanstalk.com/webapi/elevators 
WITH CONTENT BODY SAMPLE
  {
            "currentFloor": "4",
            "elevatorId": "SJCG0000"
}

PUT http://elevator-env.ap-southeast-2.elasticbeanstalk.com/webapi/elevators 
WITH CONTENT BODY SAMPLE
  {
            "currentFloor": "4",
            "elevatorId": "RONW0000"
}

GET http://elevator-env.ap-southeast-2.elasticbeanstalk.com/webapi/elevators/{ID} (returns the details of the elevator of the respective ID either in JSON or XML format)

PUT http://elevator-env.ap-southeast-2.elasticbeanstalk.com/webapi/elevators {ID}
WITH CONTENT BODY SAMPLE
  {
            "currentFloor": "6",
            "elevatorId": "RONW0000"
}

DELETE http://elevator-env.ap-southeast-2.elasticbeanstalk.com/webapi/elevators (Deletes all the contents of elevators)

DELETE http://elevator-env.ap-southeast-2.elasticbeanstalk.com/webapi/elevators/{ID} (Deletes the contents of the respective id)

