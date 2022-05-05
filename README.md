The Patient Monitoring System will be characterized as a system used to monitor physiological signs including parameters such as an electrocardiogram (ECG), respiratory signs, invasive and non-invasive blood pressure, bodytemperature, and room temperature and humidity. Understanding and validating the monitoring system is an innovation at Mhealth. can be called mhealth or mobile health. This system is used for medical and general care using cell phones. These watch frames can be used locally or remotely. Monitoring of patient relates to various situations in which patient has a comorbid condition. Patient monitoring is not another new framework in medicinal services as it was first begun in the year 1625 for checking the body temperature and pulse of 
patients. Subsequently, this framework has started to discover its utilization and 
acknowledgment for checking diverse sorts of physiological parameters and health 
related angles that are being performed as of not long ago.

We have a flutter-based front end and java spring boot-based main server and a 
node MCU server for hardware.
Java Spring boot main server is made on microservices architecture. The first layer 
is the authentication service. It authorizes any request from the server to check if it 
is a valid user. When the user will log in to the system it will send to the java spring 
boot to authenticate. If yes then it will show a successful response and an access token will be given. The access token is stored by the front-end server and is used 
for a y future login.
If it fails to pass the access token user can’t use any kind of service in the 
application.Behind the Authentication service, we have two more services namely 
medicine dispatcher service and analytics. We have three-layer of neural networks 
3 dense layers 3 hidden layers each of size 10 units.
In data analytics, we take a health dataset and predict the user's cholesterol, blood 
pressure, oximeter level, and body temp we predict the health condition and 
whether he is in good condition.
Now the Medicine reminder, If a user wants to set the medicine it will send the post 
request to the server. It will note the time in the scheduler. When the time of 
medicine approaches the main server sends a signal to the node MCU server to ring 
the reminder. Node MCU will accept the request and through 12C serial 
communication will send it to Arduino. The original message will display on LCD 
and the medicine dispatcher will move alternately
