## JobsityChallenge

###### This Backend Script uses Apache Airflow for Automatation for Transformations and ingesting a CSV File from google Drive and insert data into a Google Cloud Database that is previous configure into Google  Big Query


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


## Note
* the zip folder contains the twilio credentials,connection string, sender and receiver whatsappnumber, i am sharing this for validation for the project only.
* I configure the receiver number with my phone number because its directly atached to my twilio account, for the purpose of this test
* if another twilio account is used, the phone number of the receiver must be they own number


## Note

* for Google big query validations in another user account and instance, please change enviroment value of connection string.

## Note

* if this project requires another twilio account for test purposes I truly suggest this link:https://www.twilio.com/blog/enviar-mensaje-whatsapp-30-segundos-con-python

## Configure Variable Enviroments in Linux:

* Run Command vim .bashrc
* add enviroment variables with export command like this:

     * 1. TWILIO_ACCOUNT_SID=mysid
     * 2. export TWILIO_ACCOUNT_SID
     * 3. export PATH=$PATH:$TWILIO_ACCOUNT_SID/bin
     * 4. export TWILIO_AUTH_TOKEN
     * 5. TWILIO_AUTH_TOKEN=mytoken
     * 6. export PATH=$PATH:$TWILIO_AUTH_TOKEN/bin
     * 7. export CON_STRING
     * 8. CON_STRING =myconstring
     * 9. export PATH=$PATH:$CON_STRING/bin
     * 10. export SENDER
     * 11. SENDER=whatsappsendernumber
     * 12. export PATH=$PATH:$SENDER/bin
     * 13. export RECEIVER
     * 14. SENDER=whatsappreceivernumber
     * 15. export PATH=$PATH:$RECEIVER/bin


#####  after edit vim .bashrc with nano, save the file as follows with this command :wq!

#####  I truly recommend this video for the configuration of enviroment variables in linux : https://www.youtube.com/watch?v=NvAYH5Qu_YQ


## Configure Variable Enviroments in windows:

* --> edit enviroment variables in windows
* --> add variable name TWILIO_ACCOUNT_SID with the key sid value
* --> add variable name TWILIO_AUTH_TOKEN with the key auth value
* --> add variable name CON_STRING with the connection value
* --> add variable name SENDER with the sender number value value
* --> add variable name RECEIVER with the receiver number value value
* --> reboot your computer


######  for more information visit: https://www.twilio.com/blog/2017/01/how-to-set-environment-variables.html

###### enjoy!
