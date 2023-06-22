1. Run docker run -dp 3306:3306 -v ./conf.d:/etc/mysql/conf.d:ro -e MYSQL_ALLOW_EMPTY_PASSWORD=true -e MYSQL_USER=petclinic -e MYSQL_PASSWORD=petclinic -e MYSQL_DATABASE=petclinic mysql:8.0
2. Run docker logs -f <CONTAINER ID>, make sure MySQL is running
3. Add Environment Variables in PetClinicApp: USER_NAME=petclinic; USER_PWD=petclinic; DB_URL=jdbc:mysql://localhost:3306/petclinic
4. Start the app
5. Test the app http://localhost, make sure everything works fine
6. Stop the app
7. Run docker stop
8. Run docker remove
9. Run docker image remove mysql:8.0