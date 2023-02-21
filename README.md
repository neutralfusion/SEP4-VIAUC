# SEP4-VIAUC
System for monitoring environment for noise, temperature, humidity and CO2 in farms.

# About the Project

The administrators of Farmerama, a small pig farm in Horsens, agreed on investing into a
system which monitors the living conditions of the animals in terms of noise, temperature,
humidity and CO2. In this way, the live data and evaluations provide better supervision over
the natural conditions within the barn with the goal of enhancing the pigs’ health. In regard to
this future system need, a series of discussions and agreements were conducted by the
Product Owner, the stakeholders and the farm’s administrators. This process resulted in 50
functional and 6 non-functional requirements used by a set of actors: employees,
administrators and guests. Therefore, the main functionalities of the system are:
authentication, managing the environment related to the threshold changes which can
trigger the movements of the windows inside the barn, managing accounts, viewing
historical and latest data regarding the measurements, administering areas at choice and
managing personal profile.

The system consists of a client-server application with the client being the presentation tier,
which takes care of the user experience within the system through an Android application.
The server, responsible for handling the business logic and persisting data, consists of a
web service implementation, a gateway application and a data warehouse. The IoT devices,
that are running using FreeRTOS, are responsible for measuring data and sending it through
the LoRaWAN network which the server then receives. The communication between the IoT
devices and the server is bidirectional as the IoT devices also receive data in order to modify
measurement thresholds and these instructions are sent all the way from the Android
application through the server.

The quality of the system was concluded after a certain amount of tests were conducted.
White Box and Black Box testing was performed with an emphasis on the latter in order to
test all the use cases. According to the results, the system delivered fulfils the expectations
of the Product Owner’s and the Farmerama administration.
