# Step 4 - Sending IOT Data
   
   1. Paste the below code into the Cloud Shell to manually push data

           gcloud pubsub topics publish $TOPIC --message '{"device":"chill-1", "type":"chiller", "temp":30.3}'

           gcloud pubsub topics publish $TOPIC --message '{"device":"chill-2", "type":"chiller", "temp":29.8}'

           gcloud pubsub topics publish $TOPIC --message '{"device":"freeze-1", "type":"freezer", "temp":2.2}'

   2. Paste the below code to run a simulator to send IIOT data

           git clone https://github.com/eric-lowry/pubsub-simulator

           cd pubsub-simulator

           npm install 

          ./bin/simulator

   3. The code does the following:

Downloads the source code repository for the simulator.
Changes the directory 
Installs the prerequisite modules for the simulator
Starts the simulator which sends IIOT data every 10 seconds


Leave this running, sending data for task 5
