# Step 3 - Create a Streaming Dataflow job reading from Pub/Sub and pushing to Elastic

## **NOTE: for troubleshooting see screenshots/files in this folder**
   
   1. Enable the Dataflow API
   
   2. Paste the below code into the Cloud Shell to create a Dataflow job, making edits to the parts in RED.
   This job will read data from your BigQuery dataset and push it to Elastic.
   Enter these values by hand into the cloud shell (one by one):

               export CLOUD_ID=<< your cloud ID from step 1.13 >>
               export API_KEY=<< your API key from step 1.10 >>

   3.  To create and run a dataflow job, cut and paste the following lines into the cloud shell:

            gcloud dataflow flex-template run qwiklabs-iiot-stream-`date +%s` --template-file-gcs-location gs://dataflow-templates-us-central1/latest/flex/PubSub_to_Elasticsearch --region us-central1 --num-workers 1 --parameters inputSubscription=projects/$GOOGLE_CLOUD_PROJECT/subscriptions/$TOPIC-sub,errorOutputTopic=projects/$GOOGLE_CLOUD_PROJECT/topics/$TOPIC-errors,namespace=iiot,maxNumWorkers=1,apiKey=$API_KEY,connectionUrl=$CLOUD_ID   

