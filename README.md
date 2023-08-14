# GCP-and-Elastic
## Monitoring IOT using Google Pub/Sub and ElasticSearch
### Summary: 
  This self-paced lab walks a user through creating a IOT simulator and using GCP and Elastic to explore this data in near real time. You will do this by creating an IOT simulator that sends data to Pub/Sub, then you will use Dataflow to move this data to Elastic.

  This Lab will focus on analyzing and exploring Industrial IOT data, which can be used to improve operational efficiency, reduce costs, improve customer experience and make better business decisions.


#### Respository Structure:
  / Part 1: Elastic on GCP - Set up a trial account
  
  / Part 2: Pub/Sub set up (Topics and Subscriptions)
  
  / Part 3: Create a Streaming Dataflow job reading from Pub/Sub and pushing to Elastic
  
  / Part 4: Sending Industrial IOT Data
  
  / Part 5: Explore the data in Elastic

##### If you are doing this lab in your own environment, it's recommended to create a seperate project to islotate the work. If you are doing this lab in a Qwiklabs environment, follow the below steps:

Setup
  Labs are timed and you cannot pause them. The timer, which starts when you click ‘Start Lab’, shows how long Google Cloud resources will be made available to you.

  This hands-on lab lets you do the lab activities yourself in a real cloud environment, not in a simulation or demo environment. It does so by giving you new, temporary credentials that you use to sign in and access Google Cloud for the duration of the lab.

  **Note**: Use an Incognito or private browser window to run this lab. This prevents any conflicts between your personal account and the Student account, which may cause extra charges incurred to your personal account.

**Note**: If you already have your own personal Google Cloud account or project, do not use it for this lab to avoid extra charges to your account.

After starting your lab, copy the username, and then right click Open Google Console, then select “open link in incognito window”. The lab spins up resources, and then opens another tab that shows the Sign in page.

In the Sign in page, paste the username that you copied from the left panel. Then copy and paste the password.

Click through the subsequent pages:
  Accept the terms and conditions.
  Do not add recovery options or two-factor authentication (because this is a temporary account).
  Do not sign up for free trials.
  After a few moments, the Cloud Console opens in this tab.

Note: You can view the menu with a list of Google Cloud Products and Services by clicking the Navigation menu at the top-left.

