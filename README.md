# FunctionBlock
Arduino IDE compatible library to manage basic PLC functions and function blocks defined by json configuration file

# Purpose
The purpose of this library is to supply a configurable framework to use basic functions and objects used in plc programming to the Arduino world.
I will try to include an increasing number of functions and function blocks in this library. As this takes some time I will appreciate any help in this matter.

Configuration is privided by json file in the filesytem.
Example (Digital input on pin 2 connected to a Digita output on pin 0:

{
  "FB1": 
  {
    "DigitalInput":"1",
    "Attributes":{"Pin":2, "Period":5000 }
  },
  
  "FB2": 
  {
    "DigitalOutput":"1",
    "Attributes":{"Pin":0 },
    "Inputs":
    {"I":
      {"Q":"FB1"}
    }
  }
}

# Features
