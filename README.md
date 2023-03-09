# IOT ESP32 Firebeetle 

José Antonio López Saldaño A01710367

Emiliano Gómez Gonzalez A01710711

Cristian Chavez Guia A01710680

Axel Camacho Villafuerte A01710217

Fernando Josue Matute Soto

Ricardo Navarro Gomez

## Objective
Create a code that makes a LED blink.

## Software Used
Arduino IOT Cloud


# DEVICE SETUP

Device used: ESP32 
Model: FireBeetle-ESP32


You'll first go the the 'Devices' section' and click on the 'Add' button.
![image](https://user-images.githubusercontent.com/89211436/223789106-2002b6ad-5956-445a-adab-37f2d21e4730.png)

Then you'll set up a 3rd Party Device.
![image](https://user-images.githubusercontent.com/89211436/223789371-d736460d-ba26-441f-9d27-a3e28d176922.png)

Choose the ESP32 device, with model FireBeetle-ESP32 and click on 'Continue'.
![image](https://user-images.githubusercontent.com/89211436/223789572-91513809-7974-4bfe-aa81-66058cbdf8a7.png)

Give your device a name and click 'Next'.
![image](https://user-images.githubusercontent.com/89211436/223789841-8df91114-e607-4704-a448-f2aa3ce147fd.png)

Copy the Device ID and your Secret Key for future steps.
![image](https://user-images.githubusercontent.com/89211436/223790419-27cba670-5491-4abb-b3d3-a8f390aa6c2f.png)

Make sure to copy these and continue.
![image](https://user-images.githubusercontent.com/89211436/223790693-51bc7c36-8f4a-47cc-9407-ab31d5e8be27.png)

THE DEVICE IS SETUP!
![image](https://user-images.githubusercontent.com/89211436/223790826-801cda76-8732-45ec-bb5f-9863425e7cdf.png)



# THING SET UP

## Variables.
Go to the 'Thing' section and Create a Thing.
![image](https://user-images.githubusercontent.com/89211436/223791302-8d868575-9155-494c-b6a0-6960ab810d6e.png)

Give this thing a name and click on 'Add Variable'.
![image](https://user-images.githubusercontent.com/89211436/223791740-b21a8717-83df-4207-9f10-96700ce1fc3f.png)

For the first variable, give it the name 'blinkingTime' and assign it as an integer. Click on 'Add'.
![image](https://user-images.githubusercontent.com/89211436/223792169-ad0a404b-fc29-4c12-84b7-92e8039222de.png)

Add another variable, give it the name 'switchOn' and assign it as a bool. Click on 'Add'.
![image](https://user-images.githubusercontent.com/89211436/223792429-3202bb7a-60cd-4530-b822-7b8bef59c1bf.png)

Variables are set up!
![image](https://user-images.githubusercontent.com/89211436/223792789-2fb61736-1ab1-4507-b08f-587ae8538edc.png)



## Associated device

Click on the 'Select device' button in the 'Associated Device' section.
![image](https://user-images.githubusercontent.com/89211436/223907813-10dfadbf-efd6-4228-8c51-dd4f22ce72d2.png)

Associate the device previously set up.
![image](https://user-images.githubusercontent.com/89211436/223907911-769f0fe1-7eae-4695-a061-b3b585488e78.png)

Device is now associated!
![image](https://user-images.githubusercontent.com/89211436/223907998-2401829a-3a87-4f34-9c45-f9eece5c1f99.png)


## Network
Below the 'Select Device' section there is the 'Network' selection, were you will introduce a WI-FI network with its respective password and use your secret key to establish the connection.
![image](https://user-images.githubusercontent.com/89211436/223908277-ea45e28d-c858-47f4-af65-cfba23e87da3.png)


## Sketch
To read the full arduino code, check the jointed file in this repository. 

## Sketch error
In order to send the code correctly to the ESP32 via USB port, you need to have the Create Agent installed in your computer.
When entering the 'Sketch' section, this message will appear, so follow the instructions said there.
![image](https://user-images.githubusercontent.com/89211436/223909764-e39e96c9-7c10-4256-bacc-c6dfb4172cd9.png)


## Sketch Compilation
To verify that your code is correct, click on the checkmark button to start compiling.
![image](https://user-images.githubusercontent.com/89211436/223909952-780e80fc-b776-4c83-9b61-2ba07f556844.png)

This can take a while...
![image](https://user-images.githubusercontent.com/89211436/223910031-cd5eca0c-0687-4589-bc5f-0a73a79e685c.png)

If everything is correct, arduino will tell you so.
![image](https://user-images.githubusercontent.com/89211436/223910112-7a0a8b47-edd7-4e66-9ee4-03af12aaae73.png)

NOTE: You can also do this by opening the full editor.
![image](https://user-images.githubusercontent.com/89211436/223910272-a4e7dbcb-2244-4942-8a73-02062c8eccf9.png)



# ESP32 CONFUGURATION

## Dashboard
For this part you'll go to the Dashboard section of your project
![image](https://user-images.githubusercontent.com/89211436/223786403-e3e91d80-0eba-4243-a9b2-859f55999a19.png)

Add a Dashboard and name it
![image](https://user-images.githubusercontent.com/89211436/223786681-c87cc644-4ba2-489d-b679-ceab08e2f293.png)

Add widgets with the 'Add' button. 

Add 'Switch' and name it like the 'switchOn' variable.
![image](https://user-images.githubusercontent.com/89211436/223787198-9f2c3696-b84c-41e1-8b4e-611d3a44b39b.png)

Link it to the 'switchOn' variable with the 'Link Variable' button.
![image](https://user-images.githubusercontent.com/89211436/223787422-eb7490c9-c468-4690-8752-356d45071005.png)

Press the 'DONE' button.
![image](https://user-images.githubusercontent.com/89211436/223787596-2a1e3630-1813-4787-8f5d-0210a38036b6.png)


Repeat the same proccess for the 'Value' widget.
![image](https://user-images.githubusercontent.com/89211436/223787877-326ac37c-64dc-44be-935b-fd7643a95e53.png)

![image](https://user-images.githubusercontent.com/89211436/223787967-08d4b542-679c-403d-b0e6-1573de76b644.png)

![image](https://user-images.githubusercontent.com/89211436/223788061-37b084b0-d7dc-49cb-991d-0789ef83c013.png)


Widgets are added!
![image](https://user-images.githubusercontent.com/89211436/223788209-0044f20c-bf5d-45ad-8bdd-e04ecc9a8eea.png)



# Connection
After widgets are addes, compile the code again and send it to the ESP32 via USB port. Depending on the time you put on the value widget, it will be the time the LED stays on or off. Since the widget is in miliseconds, to have it on for a minute, set it to 60000, it will then be off for another minute and so on. 








