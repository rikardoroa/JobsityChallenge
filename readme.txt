This Backend Script uses Apache Airflow for Automatation 
for Transformations and ingesting a CSV File from google Drive and insert data
into a Google Cloud Database that is previous configure into Google 
Big Query


#Scalability -> This Script uses a google big query ingestion, so it can be added more that 100 millions registers

#Automation ->this script Uses Apache Airflow, the orchestation of this script is  
daily for all task in the script

#Notification -> this script uses Twilio Libraries for whatsapp messaging,
so, every time that the records are ingested in the database daily, the users receive a notification
in whatsapp

#SQL --> all data is ingested in Google Cloud in Big Query enviroment

#The trips are grouped by hour, region, average and by origin and destination coord

Note: Prior using the whatsapp messages, in the twilio account( I used my personal account)
need to be configure the phone number of the user. for the moment i have mine.