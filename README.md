This code will run the docker service, assuming the pkl files are already present.

Run these commands

docker build -t titanic_serv .

docker run -p 8001:8000 titanic_serv

Use the following URL in POSTMAN

localhost:8001/predict

Use the below body 

{"Pclass": 1,
    "Sex": 0,  
    "Age": 35,
    "SibSp": 2,
    "Parch": 2,
    "Fare": 25}
