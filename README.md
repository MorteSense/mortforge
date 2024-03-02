# Mort Forge

## Software Class Diagram

![image](https://github.com/MorteSense/mortforge/assets/22685770/c9c8f86e-ad95-4d6b-9e6c-d4e7a2748b4c)

The Class Diagram represents the relationships between various classes in the Microwave Motion
Security System with SMS Notifications. The User class is associated with the MicrowaveSensor
class, which is responsible for detecting motion. The SMSService class is associated with the
Database class, which is used to store data related to the SMS services used to send SMS
messages to the user. The MicrowaveSensor class is associated with the Notification and
SMSService classes, which are responsible for sending notifications and SMS messages to the
user when motion is detected. These associations enable the MicrowaveSensor to trigger the
Notification and SMSService classes to send a notification and an SMS message
to the user, respectively.

The Database class is associated with the Notification, NotificationLog, SMSService,
SMSServiceLog, and SensorLog classes, which are used to store data related to notifications,
SMS services, and sensor logs. The Notification and SMSService classes have a one-way
association with the Database class, indicating that they can use the Database to store data
related to the notifications and SMS services sent to the user. Additionally, the Notification
and SMSService classes have composition relationships with the NotificationLog and
SMSServiceLog classes, respectively. These composition relationships indicate that a
Notification or a SMSService ``has-a'' relationship with their respective log tables, and the
log tables cannot exist independently of the Notification or SMSService.

Finally, the SensorLog class has a one-way association with the MicrowaveSensor class, which
indicates that it can store data related to the logs of the microwave sensors used for
detecting motion. Overall, the Class Diagram demonstrates the flow of information and data
between the various classes and tables in the system, providing a comprehensive representation
of the Microwave Motion Security System with SMS Notifications.

In this way, the system can detect motion using the MicrowaveSensor, send notifications
and SMS messages to the user using the Notification and SMSService classes, respectively,
and store data related to these events using the Database, NotificationLog, and
SMSServiceLog tables.

## Notes

1. Requirements.txt
2. Redis server
3. Python Flask
4. MySQL
5. AWS
6. Twilio API

Additional Notes:
* The backend solution includes a requirements.txt file outlining the necessary dependencies.
* A Redis server is used for caching and session management.
* Python Flask is the chosen web framework for the backend.
MySQL is utilized for data storage.
* AWS services are employed for various functionalities.
* The Twilio API is integrated for communication purposes.
