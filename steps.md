1. Go to db-postgres folder
   Run 
   kubectl apply -f .

2. Go to web-pgadmin folder
   Run 
   kubectl apply -f .

3. setup telemetry table in postgres using query:
   Run 
   kubectl port-forward svc/svc-web-pgadmin 80:80
   open localhost:80 in browser
   Add the database: name indri-db, user : admin, password : Passw0rd
   look for indri-db > right click > add query >
   Copy the query from DB-query-Schema and paste it and run the query (F5)
   Test, if you see the telemetery table.

4. Go to app-simulator folder
   Run 
   kubectl apply -f .

5. Go to app-ingest folder
   Run 
   kubectl apply -f .

6. Go to app-backend folder
   Run 
   kubectl apply -f .

7. Go to app-frontend-ui folder
   Run 
   kubectl apply -f .

8. Go to web-pgadmin folder
   Run 
   kubectl port-forward svc/svc-app-frontend-ui 80:80
   Open browser and test the application
   open localhost:80
   userID : admin@nsdobal.online
   Password : Welcome
   