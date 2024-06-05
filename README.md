# STM32F103C6x UART SPI Communication
This project demonstrates communication between two STM32F103C6x microcontrollers (MCUs) <br>
 using  the Serial Peripheral Interface (SPI) protocol and Universal Asynchronous Receiver Transmitter (UART). <br> 
One MCU acts as the master (MCU1) and the other as the slave (MCU2). <br>
 Data is sent from a terminal connected to MCU1's UART, transmitted via SPI, and displayed on the terminal connected to MCU2's UART.

**Project Overview:**

* **Hardware:**
    * Two STM32F103C6x development boards
* **Communication Protocol:**
    * SPI: Used for data transfer between MCUs
    * UART: Used for communication between terminals and MCUs
* **Data Flow:**
*   Terminal1 <-----> USART1 : MCU1 : (SPI1 Master) ---> (SPI2 Slave) :MCU2: USART2 ---> Terminal2
    1. User sends a character through the terminal connected to MCU1.
    2. MCU1 generates an interrupt upon receiving the character on its UART.
    3. MCU1 transmits the received character to MCU2 using SPI.
    4. MCU2 generates an interrupt upon receiving data from SPI.
    5. MCU2 displays the received character on its UART terminal.


**Features:**

* Master-slave SPI communication between two STM32F103C6x MCUs.
* UART communication for user interaction with each MCU.
* Character echo functionality from terminal to terminal.

**Developed and Simulated in:**

* Proteus Design Suite

**Getting Started:**

The project files (source code, schematics, etc.) are required to run this project. found in the Driver Folder. 

**Simulation**


### Terminal1 <-----> USART1 : MCU1 : (SPI1 Master) ---> (SPI2 Slave) :MCU2: USART2 ---> Terminal2
![STM32F103C6x UART SPI Communication](https://github.com/ArsanyMounir/STM32F103C6x_UART_SPI_Communication/blob/main/Proteus.gif)
