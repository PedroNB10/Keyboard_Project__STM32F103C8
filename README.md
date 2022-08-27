# Keyboard_Project__STM32F103C8


 
===============   Setup Pins   =============== <br />

![My Image](setup_pins_configurations.png)

===============   Observations   =============== <br />
In case you change the .ioc MX, the usbd_hid.c and usbd_hid.h  in this local : \Keyboard_Project__STM32F103C8\Middlewares\ST\STM32_USB_Device_Library\Class\HID\Src

and this \Keyboard_Project__STM32F103C8\Middlewares\ST\STM32_USB_Device_Library\Class\HID\Inc respectively, are going to regenrate the standard code, and you are going to miss every configuration you have made in this two places.

===============   Important places to code in .main   ===============
<br />

/* USER CODE BEGIN PV */ <br />
//Here you declare global variables <br />
/* USER CODE END PV */ <br />
<br />
<br />
/* USER CODE BEGIN PFP */ <br />
Functions Declaration (helps to remove warnings of program) <br />
e.g. : <br />
void function(); <br />
/* USER CODE END PFP */ <br />
<br />
<br />
/* USER CODE BEGIN WHILE */ <br />
while (1) <br />
{ <br />
//Here comes the code that´s gonna work in loop <br />

 /* USER CODE BEGIN 3 */ <br />
 
 //If you are using STM32 as a HID(Human Interface Device) you should put your code that is going to repeat inside this tag <br />
 
  /* USER CODE END 3 */ <br />

<br />
 /* USER CODE END WHILE */ <br />
 <br />
<br />
/* USER CODE BEGIN 4 */ <br />
Here you put the functions that you are going to use or call <br />
e.g. : <br />
void function() { <br />
//CODE <br />
} <br />
<br />
/* USER CODE END 4 */ <br />

