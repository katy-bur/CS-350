# CS-350

# Summarize the project and what problem it was solving.
In this project we were able to create a thermostat with the interrupt function when it reached the needed temperature. Interrupt start was initial temperature and then two buttons one was increasing the set temperature and the other one is decreasing. When I increased the set temperature and the init temperature in the room was below the indicator showed red LED and the heat was ON. Once the temperature raised to the set temperature the heat was off and led was off. To set up the buttons for increase and decrease of temperatures gpioButtonFxn0 and 1 were used. Button 0 was used to increase the value of temperature by 1 and button 1 was used to decrease the value by 1. 


Each peripheral used during the project will be described below. The thermostat must support I2C peripheral, GPIO peripheral, and UART peripheral. I2C is an inter-integrated circuit that implements half duplex function and uses 2 pins. I2C is synchronous serial communications interface. UART is a universal asynchronous receiver-transmitter that also uses 2 pins like I2C, but it is asynchronous, serial data transmission between the devices. GPIO is a general-purpose input and output peripheral. GPIO controls 16 pins. In this code we were able to use standard UART drivers code to init the driver and to fully configure the driver. For I2C we called the function initUART before calling initI2C, then we configure and opened the driver. 


There is a need to connect the thermostat to the cloud by using Wi-Fi. To make sure that the thermostat is connected to the Wi-Fi we will use IoT. And from TechTarget article “IoT devices share the sensor data they collect by connecting to an IoT gateway or other edge device where data is either sent to the cloud to be analyzed or analyzed locally.” IoT device will collect data, then it will take the data by using the hub or IoT gateway to collate and transfer the data, and then it will analyze data and take further action by using user interface or aback end systems. The three layers of IoT are perception, network, and application. 



# What did you do particularly well?


I learned about best coding practicies and did pretty well following them. As of best coding practices for embedded C there are a few important ones that should be followed by everyone who writes code for embedded systems. There is a need to follow the rules to make the code readable and reliable. A few examples for coding standards best practices according to Richard Bellairs (2018), “Prioritize Coding Rules, Plan for Rule Deviations, Educate Programmers.” Prioritize Coding Rules is an important rule. If the code has a lot of errors and it doesn’t fit into coding rules the code isn’t supposed to be released. When the code has a few errors and can be fixed it should be a low priority in the production. Making priorities for the production can be helpful in the development. Plan for Rule Deviations is coming from a personal experience from my work in IT field. Coding rules are always a priority, but they don’t always fit and they need a walk around. There must be a list of ules in every organization about documentations of deviations for the code. From legal perspective every change must be researched, documented, and tested. And the last important step from the list is going to be Educate programmers. We should be able to provide the documentation with the specific examples to educate programmers. We should give a lot of extra information for how things are configured in a software design that is created. It will save time and money for the training for new people. 

# Where could you improve?


There is no place for perfection and I decided to move to cybersecurity in my future. I think I will be learning more Linux and security tools. I am looking forward to this.

# What tools and/or resources are you adding to your support network?


There are 3 types of microcontrollers to discuss Freescale, TI, and Microchip. The new microcontrollers should give us more freedom to develop new electronic products. Microchip’s  technology “8-bit direct LCD-drive microcontroller features 64-128 KB Flash and 4 KB RAM” information is taken from the DesignNews what gives microchip empowerment over TI. TI on the other hand starts at 38 pins and 32-but microcontrollers with a little price less than two dollars per unit. TI microcontrollers are candidates for automotive applications. Freescale microcontrollers according to DesignNews “delivers up to 1.3-GHz performance within a sub-10-W power envelope. The device's integrated design allows for a single-chip solution, consolidating network processing and control processing functions.”
The board used for this project TI CS3220 LaunchPad connects to the UART, SPI, I2C servers. This board is able to connect to the Wi-fi and can transmit the data on the online server to allow multiple users access the data and set the thermostat. 


# What skills from this project will be particularly transferable to other projects and/or course work?


Coding best practicies will be the most notable one for me. One of the most common pitfalls in embedded C coding practices that I see is making a code temporarily as a comment to disable, then forgetting about that line and never coming back to it. Nested comments are allowing the risk for snippets of code to be complied. The next one is putting in a lot of empty space. It makes it very hard to find bugs and errors in the code. One more that I faced a few times before is a comma operator and there is a risk that complier will misunderstand the comma. From the Michael Barr article keyword “The upside of using const as much as possible is compiler-enforced protection from unintended writes to data that should be read-only.” In his article he shows many more different keyword examples that can cause issues in C coding for embedded systems. 




