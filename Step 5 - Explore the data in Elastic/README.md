# Step 5 - Explore the data in Elastic

## **NOTE: for troubleshooting see screenshots/files in this folder**

   1. Go to 'Discover'

   2. Click ‘Create a data view’

   3.  Name the dataview (for example 'iiot'), add an Index pattern (logs-gcp.pubsub*) and a TimeStamp field (@timestamp) from the dropdown
    Then click “Save data view to Kibana”

   4. Data should stream in, see image in file for comparison

   5. Expand one of the IOT messages to view the format and fields available
    Press 'X' to close the expanded document

   6. Click the main hamburger menu and then select Dashboard

   7. Click "Create dashboard" and then click "Create Visualization"

   8. Drag and drop the field "temp" on the canvas. "temp" is the temperature measurement for the device

   9. Filter the data to a single device named "freeze-1", by typing "device" in the search bar and selecting "freeze-1" and clikc the "update" button:

   10. Change the visualization type to "Line"

   11. Change the vertical axis to from "Median of temp":

   12. Change it to "Last value" and click "Close"

   13. Click "Save and return" to save the visualization

   14. Add a title and resize the visualization

   15. Click the gear/settings symbol in the top right corner to clone the panel and edit for second freeze

   16. Edit tht title to make it "Freezer 2", then edit the filter

   17. Change the filter from "freeze-1" to "freeze-2" and click "Update"

   18. Click "Save and return"

   19. Adjust the dashboard to the view you would like

   20. Save and name the dashboard

# Congrats!!! You've finished the lab
## In this lab, you have: Set up an Elastic on GCP environment
Created Pub/Sub Topics and Subscriptions
Created a Streaming Dataflow Job
Created a IIOT simulator that sends data
Explored the live data in Elastic

