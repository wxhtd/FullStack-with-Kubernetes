# FullStack-with-Kubernetes
MongoDB + Python Flask Web Framework + REST API + GKE
Signature Project: MongoDB + Python Flask Web Framework + REST API + GKE 
Review the concepts
MongoDB 
REST API 
Python Flask Web Framework 
Project Implementation
This project uses the above techniques:
Pods --- to run 2 applications
Pod 1: Student Records
GKE
Pod 2: bookstore
MongoDB + Python Flask Web Framework + REST API + GKE
Service --- for outside access to the application
Persistence Volumes --- to store the data with MongoDB
Ingress ---- to expose both applications under the same domain but different path
Pod 1: student records
curl cs571.project.com/studentserver/api/score?student_id=11111
Pod 2: bookstore
curl cs571.project.com/bookshelf/books
ConfigMaps ---- to store MongoDB service address, in case MongoDB is down and restarts with a different service address, and with ConfigMaps, we don't need to build the docker image again with the new address

