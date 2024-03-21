# Flight-Reservation-Automation-Testing
# Project Structure

# ----- Software Testing lifecycle -----

# Requirement Analysis
# Test Planning
# Test Case Development
# Test Environment Setup
# Test Execution
# Test Cycle Closure

# Flight Reservation UI Journey
1. Customer Registration
2. Registration Confirmation
3. Flight Search    
4. Flight Select 
5. Flight Confirmation

mvn clean package -DskipTests

docker build -t=atharvahiwase7/flightreservation .

docker run -it -v D:/FlightReservationProject/flightreservation/result:/home/flightreservation/test-output atharvahiwase7/flightreservation

java -Dselenium.grid.enabled=true -Dselenium.grid.hubHost=192.168.0.104 -cp "libs/*" org.testng.TestNG test-suites/flight-reservation.xml

we can delete the images which are called as None- 
To get rid of none named images hit the below command
docker system prune -f