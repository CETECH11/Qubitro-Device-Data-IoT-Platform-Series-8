# Qubitro-Device-Data-IoT-Platform-Series-8

![alt text](https://hackster.imgix.net/uploads/attachments/1595875/image_TVv0Hcp8Eu.png?auto=compress%2Cformat&w=740&h=555&fit=max)
Qubitro is an IoT (Internet of Things) platform that provides tools and services for connecting, managing, and analyzing IoT devices and data. It provides a cloud-based platform where users can securely connect their IoT devices and collect data from sensors and actuators.

It supports a wide range of communication protocols and provides device management capabilities, monitoring device data, linking with third-party webhooks, and creating rules to trigger based on conditions, etc. All of it with a Great UI ❤
To get started with Qubitro, we will first need to create an account. Go to the Qubitro website (https://www.qubitro.com/) and click on the "Sign Up" button. You will be prompted to enter Full Name, Email Address,Country, and password to create your account.

Once, we have created the account, we can log in from https://portal.qubitro.com/login. However, we shall automatically be logged in to our account.

![alt text](https://hackster.imgix.net/uploads/attachments/1595877/image_jFN41wk7w7.png?auto=compress%2Cformat&w=740&h=555&fit=max)

Once you have logged in, you will be prompted to create a project. Enter a name for your project and mention a description for your project.

Add Devices
Next, you will need to add devices to your application. Go to the Project (if not already open), there we can see a button [+ New Source]. From this section, we will have 3 major sections -

1. Communication Protocol-With a prompt to choose between LoRaWAN, MQTT, & Cellular. We can choose the protocol that best suits our use-case.
I choose MQTT to get started with the platform basics. And since I shall be using Arduino IDE for programming the board, I went ahead with the MQTT Broker (Qubitro has its own broker - we shall see it in the upcoming section). In case you wish to know how the Toit platform works, you can check my Tutorial on Toit.io
2. Device Details-I shall be using an ESP32 Dev Board, and therefore entered the details as per the image below -
3. Credentials-In the next step, we receive credentials, to connect to the MQTT Broker. We can use this detail to connect to the broker as a client - to Publish or Subscribe.

Now that we have the server, port, username and password we are all ready to send data to the Qubitro Cloud. Copy these details in a safe place (We can view them later in the device settings as well though)

![alt text](https://hackster.imgix.net/uploads/attachments/1595481/image_s00pP05CfN.png?auto=compress%2Cformat&w=740&h=555&fit=max)

Once you have configured your devices, you can start collecting data. Qubitro provides a range of tools for data collection and analysis, including real-time data visualization, data logging, and data filtering.

We shall upload a code on ESP32 using Arduino IDE to send data to Qubitro
Now that we were able to fetch for real-time data from the ESP32 board and view it on the table of Qubitro. Let us use the visualization feature to plot a graph of the data. Trust me, it takes seconds to setup the whole thing.

Go to Dashboards, and create a New Dashboard. Give it a name.
Once created, open it and go to Edit > Add Widget > Charts.
Click on the new widget > three dots (settings) > Customization.
Accordingly, select the data source, chart type and colour for data variables. Follow the below images for reference, and final Graph.

![alt text](https://hackster.imgix.net/uploads/attachments/1544797/pcbway_55Vl7NMRFG.JPG?auto=compress%2Cformat&w=740&h=555&fit=max)

You must check out [PCBWAY](https://www.pcbway.com/) for ordering PCBs online for cheap!

You get 10 good-quality PCBs manufactured and shipped to your doorstep for cheap. You will also get a discount on shipping on your first order. Upload your Gerber files onto PCBWAY to get them manufactured with good quality and quick turnaround time. [PCBWay](https://www.pcbway.com/) now could provide a complete product solution, from design to enclosure production. Check out their online Gerber viewer function. With reward points, you can get free stuff from their gift shop.
