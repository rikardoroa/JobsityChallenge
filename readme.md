## JobsityChallenge

###### This Backend Script uses Apache Airflow for Automatation 
###### for Transformations and ingesting a CSV File from google Drive and insert data
###### into a Google Cloud Database that is previous configure into Google  Big Query


* Scalability -> This Script uses a google big query ingestion, so it can be added more that 100 millions registers

* Automation ->this script Uses Apache Airflow, the orchestation of this script is  
daily for all task in the script

* Notification -> this script uses Twilio Libraries for whatsapp messaging,
so, every time that the records are ingested in the database daily, the users receive a notification
in whatsapp

* SQL --> all data is ingested in Google Cloud in Big Query enviroment

* The trips are grouped by hour, region, average and by origin and destination coord

## Note
* Prior using the whatsapp messages, in the twilio account( I used my personal account) need to be configure the phone number of the user. for the moment i have mine.


## Note
* If you Want be receiver from notifications just add the contact number  +415523886 from twilio and then write the msj "join easy-composition" via whatsapp


## Configure Variable Enviroments in Linux:

* Run Command vim .bashrc
* add enviroment variables with export command like this:

 *TWILIO_ACCOUNT_SID=mysid*
 *export TWILIO_ACCOUNT_SID*
 *export PATH=$PATH:$TWILIO_ACCOUNT_SID/bin*
 *TWILIO_AUTH_TOKEN=mytoken*
 *export TWILIO_AUTH_TOKEN*



## Configure Variable Enviroments in windows:

* --> edit enviroment variables in windows
* --> add variable name TWILIO_ACCOUNT_SID with the key sid value
* --> add variable name TWILIO_AUTH_TOKEN with the key auth value
* --> reboot your computer


######  for more information visit: https://www.twilio.com/blog/2017/01/how-to-set-environment-variables.html
