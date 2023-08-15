# Step 2 - PubSub setup

## **NOTE: for troubleshooting see screenshots/files in this folder**

  1. Open the Cloud Shell by clicking the box in the top right corner.

  2. Paste the below code into the Cloud Shell to create a new bucket and copy data from an existing bucket:
  
    export TOPIC=qwiklab-test
    gcloud pubsub topics create $TOPIC
    gcloud pubsub topics create $TOPIC-errors
    gcloud pubsub subscriptions create $TOPIC-sub --topic=$TOPIC

The first command sets the topic equal to qwiklabs-test. The next two gcloud commands will create two pubsub topics, ‘qwiklab-test’ and ‘qwiklab-test-errors’.

The last command will create a subscription ‘qwiklabs-test-sub’ that subscribes to the first topic. Go to PubSub in the GUI to confirm that the Topics and Subscription were created
