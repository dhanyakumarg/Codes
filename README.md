# Research Internship on VSDSquadron Mini RISC-V Development Board
**About:**
The internship is based on RISC-V Development Board(VSDSquadron Mini),which is a flagship product of VLSI System Design.It is a 4-week internship program on RISC-V.
The program has three types of internship
1.Beginners
2.Intermediate
3.Advanced.
My internship is on Beginner(VLSI), which is on VLSI.         
For more details of company  visit [Company's Website](https://www.vlsisystemdesign.com/).

I'm dhanyakumar g

I am a passionate third-year student pursuing a degree in Electronics & Communication Engineering. My academic journey has fueled my interest in exploring the intricacies of embedded systems, PCB layout & design, and various hardware components.

🎓 Electronics & Communication Engineering Student | 3rd Year

🏫 Mangalore Institute of Technology & Engineering

📧 ddhanyakumarg@gmail.com 

## VSDSquadron Mini RISC-V Development Board     ![image1](https://github.com/sanjaypk16/VSDSquadron-RISCV/assets/129313628/27128265-69df-4725-bc1e-84f6475f907f)
**Board Specifications** 

|   Board   |   Name   | Description                |
| :-------- | :------- | :------------------------- |
|           |       SKU| VSDSQM                     |
| Microcontroller| CH32V003F4U6 chip with 32-bit RISC-V core based on RV32EC instruction set |  |
| USB connector | USB 2.0 Type-C |  |
|   Pins  |   Built-in LED Pin  | 1X onboard user led (PD6)               |
|   | Digital I/O pins  | 15              |
|     |   Analog I/O pins  | 10-bit ADC, PD0-PD7, PA1, PA2, PC4              |
|      |   PWM pins  | 14              |
|    |   External interrupts  | 8 external interrupt edge detectors, but it only maps one external interrupt to 18 I/O ports              |
|  Communication  |   USART   | 1x, PD6(RX), PD5(TX)               |
|     |   I2C   |1x, PC1(SDA), PC2(SCL)           |
|      |  SPI   | 1x, PC5(SCK), PC1(NSS), PC6(MOSI), PC7(MISO)           |
|      |   Programmer/debugger | Onboard RISC-V programmer/debugger, USB to TTL serial port support           |
|   Power   |  I/O voltage  | 3.3 V            |
|      |   Input voltage (nominal)  | 5 V          |
|      |   Source Current per I/O Pin | 8 mA              |
|      |   Sink Current per I/O Pin | 8 mA             |
|    Clock speed  |   Processor  | 24 MHz             |
|   Memory   |  SRAM  | 2kb onchip volatile sram,16kb external program memory        |


 For board information [Click here for board link](https://www.vlsisystemdesign.com/vsdsquadronmini/)

This repository is mainly for documentation of all the progress
## Progress Report  

------------------------------------------------------------------------  


### 1st Meeting - The first online meet was held on 16th of Feb 2024 @6PM
Description:Steps to be followed for software installation.

<details>
    <summary> TASK 1 </summary>

Based on the internship type different task were assigned. 

TASKS   
1.install Yosys
2.install iverilog
3.install gtkwave  

### To install git


``` sudo apt install git-all ```

## Screenshots

#### git
```bash
  sudo apt install gtkwave
```

![Screenshot from 2024-02-23 11-49-02](https://github.com/dhanyakumarg/vvssdd/assets/132377400/7c8797e1-5b80-4bbe-9a18-b95677e27156)



#### iverilog

```bash
  sudo apt-get install iverilog
```

![Screenshot from 2024-02-23 11-50-49](https://github.com/dhanyakumarg/vvssdd/assets/132377400/3b525fa9-11cf-469a-b2ee-8451df09ca09)


#### git

```bash
  sudo apt-get install git 
```

![Screenshot from 2024-02-23 11-53-28](https://github.com/dhanyakumarg/vvssdd/assets/132377400/c999ba1b-b1f5-4fec-984c-2dc64012c969)



#### vim

```bash
  sudo apt install vim
```




![Screenshot from 2024-02-23 11-46-24](https://github.com/dhanyakumarg/vvssdd/assets/132377400/49069ca5-cd8c-4975-a38a-ea36e03ec277)





#### yosys

```bash
  yosys
```
![Screenshot from 2024-02-23 11-46-01](https://github.com/dhanyakumarg/vvssdd/assets/132377400/864e7fcd-ef07-44c6-a9ce-18f8657f554b)

</details>

-----------------------------------------------------------------------------------------------------------------------------------------------------------------
### 2nd Meeting - The second online meet was held on 20th of Feb 2024 @6PM
Description: Block diagram and identify input ports, input waveforms, output ports and output waveforms.  

<details>
    <summary> TASK 2 </summary>
Tasks  
1.To create a block diagram of the respective project  
2.To identify input ports, input waveforms, output ports and output waveforms  

### Synchronous First in First Out for Memory Storage and Processing  

**Introduction**: 

Synchronous First In First Out (FIFO) is a fundamental data storage and processing mechanism widely employed in digital systems to manage the orderly flow of data. It ensures that data is processed in the same sequence it was received, making it essential for applications where timing and order are critical.  

**Applications**:  

1.**Communication Interfaces:** Synchronous FIFOs are vital in communication protocols like UART and SPI, buffering data between devices with different clock domains to ensure synchronized data transfer.

2.**Digital Signal Processing (DSP):** In DSP applications, synchronous FIFOs manage data flow between processing stages, maintaining the sequence integrity necessary for accurate signal processing.

3.**Memory Interfaces:** They serve as interfaces between memory modules operating at varying speeds or utilizing different protocols, facilitating efficient data transfer and access while preserving order.  

**Block Diagram**  


# Synchronous First In First Out for Memory Storage and Processing
![Synchronous FIFO pdf](https://github.com/avinashjaiswal1598/Risc-V-mini/assets/160040323/f2cc94e1-feac-4f9c-bbbe-b52f01479df5)


**Input and Output Waveform**  
![Time diagram for Synchronous FIFO](https://github.com/avinashjaiswal1598/Risc-V-mini/assets/160040323/63bb283d-c5e0-4d50-a72e-49231bda283b)

</details>  

----------------------------------------------------------------------------------  
### 3rd Meeting - The third online meet was held on 22nd of Feb 2024 @6PM
Description: To know about gtkwave, Verilog and generate the waveform.
<details>
    <summary> TASK 3 </summary>
Tasks  
1.To know about gtkwave and iverilog   
 
2.To generate waveform

**GTKWave**  
GTKWave is a waveform viewer for Verilog simulation results, enabling visualization of signals over time. 

**iverilog**  
Icarus Verilog (iverilog) is a free Verilog simulation and synthesis tool, useful for compiling and simulating Verilog designs, often paired with GTKWave for waveform viewing.

### **Steps to generate waveform using gtkwave and iverilog** ###

1.Cloning my gitub repository  
``git clone https://github.com/sanjaypk16/VSDSquadron-RISCV.git`` 


![image](https://github.com/dhanyakumarg/vvssdd/assets/132377400/a06bd41c-172a-4796-96ef-ecebcc3926c1)


2.Simulating iverilog  
``cd VSDSquadron-RISCV/``            where **VSDSquadron-RISCV/** is my repository  


``iverilog fifo.v fifo_tb.v``  

Generating dump file  
``./a.out``  







3.To get waveform  
 ```gtkwave dump.vcd``` 
 
### **Waveform** ###



![verilog files](https://github.com/dhanyakumarg/vvssdd/assets/132377400/4b0fa0f4-b2e9-40fd-a11a-83aa2abf85eb)

</details>

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------  
### 4th Meeting - The fourth online meet was held on 27th of Feb 2024 @6PM    

Description: Generating the waveform with the actual code and with netlist. Verifying both the waveform

<details>
    <summary> TASK 4 </summary>  


  
**To invoke yosys**   

``yosys```  
where VSDSquadron-RISCV is my folder  

**To read the library** 

``read_liberty -lib ../../sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib``

![WhatsApp Image 2024-02-29 at 6 38 00 PM](https://github.com/dhanyakumarg/vvssdd/assets/132377400/06e8997f-6576-423f-b1ea-2bd4681519bf)

**Reading the design**


```read_verilog fifo.v```  

where fifo is the module name of the design code

![WhatsApp Image 2024-02-29 at 6 38 00 PM (1)](https://github.com/dhanyakumarg/vvssdd/assets/132377400/252b52f1-df71-4a51-b2bc-c2a1e709322b)

**Synthesizing the module**

``` synth -top fifo ```    

where fifo is the module name of the design code 
![WhatsApp Image 2024-02-29 at 6 38 00 PM (2)](https://github.com/dhanyakumarg/vvssdd/assets/132377400/d3000fa0-ecb9-478c-af61-de5fc736c197)

 **To generate netlist**  

``` abc -liberty ../../sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib```

![WhatsApp Image 2024-02-29 at 6 38 00 PM (3)](https://github.com/dhanyakumarg/vvssdd/assets/132377400/9596105c-8cd8-4223-abd9-8ad70b5c7e7c)

**To write the netlist**  
`` write_verilog fifo_netlist.v`` 



-noattr is used to get simplified version of netlist file  

``` write_verilog -noattr fifo_netlist1.v```  


```flatten```

![WhatsApp Image 2024-02-29 at 6 38 01 PM](https://github.com/dhanyakumarg/vvssdd/assets/132377400/fd16df67-d7cc-418f-8ecc-d877cba746fc)



```show```  

**To open the netlist**  


```!gvim vend_netlist1.v```  


![WhatsApp Image 2024-02-29 at 6 38 02 PM](https://github.com/dhanyakumarg/vvssdd/assets/132377400/320e9d53-098b-4e88-ac0b-0c00d6b33958)

**Opening the netlist file**   

![WhatsApp Image 2024-02-29 at 6 38 02 PM (1)](https://github.com/dhanyakumarg/vvssdd/assets/132377400/bd26e91e-108d-456e-9ee1-ee02f10f44a9)

![WhatsApp Image 2024-02-29 at 6 38 07 PM](https://github.com/dhanyakumarg/vvssdd/assets/132377400/70fdb7ab-bca7-493f-8e5d-4ac3e1ea1cf4)

**To verify whether netlist will match with the design**  

```iverilog netlist1.v fifo_tb.v```   

```./a.out```  

``` gtkwave dumpfile.vcd```


![WhatsApp Image 2024-02-29 at 6 38 07 PM (1)](https://github.com/dhanyakumarg/vvssdd/assets/132377400/396fbed1-df73-4d2a-943c-0aaa3d76bc49)


</details>


-------------------------------------------------------------------------------------------------------------------------------------------------  

![WhatsApp Image 2024-02-29 at 6 38 08 PM](https://github.com/dhanyakumarg/vvssdd/assets/132377400/2ae39b06-5a67-4f02-8bf7-111678112a96)

![WhatsApp Image 2024-02-29 at 6 38 08 PM (1)](https://github.com/dhanyakumarg/vvssdd/assets/132377400/68b0b54c-a01e-422d-a325-bb2958b065b5)

![WhatsApp Image 2024-02-29 at 6 38 09 PM](https://github.com/dhanyakumarg/vvssdd/assets/132377400/881dbe74-f315-4a76-8611-f4e58f3f6ae6)

![WhatsApp Image 2024-02-29 at 6 38 09 PM (1)](https://github.com/dhanyakumarg/vvssdd/assets/132377400/bb2d31b7-562f-4688-b18a-2007108894e0)

### 5th task - The fifth task  was given on 1st of March 2024  

Description:  To simulate the waveform with the given design code and netlist.  



<details>
    <summary> TASK 5 </summary>  


**Cloning  gitub repository**    

```bash
  $  read_liberty  -lib ../lib/sky130_fd_sc_hd__tt_025C_1v80.lib
```

![WhatsApp Image 2024-03-21 at 2 09 22 PM](https://github.com/dhanyakumarg/vvssdd/assets/132377400/794c2920-2fcc-4d81-9965-f6c3962a8df8)

<br />
<br />
<br />

```bash
  $  read_verilog good_mux.v
```

![WhatsApp Image 2024-03-21 at 2 09 22 PM (1)](https://github.com/dhanyakumarg/vvssdd/assets/132377400/94f5a2ea-c49c-43c6-a2d1-1e8f613868f2)

<br />
<br />
<br />


```bash
  $  synth -top good_mux
```<br />
<br />
<br />

```bash
  $  show
```

![WhatsApp Image 2024-03-21 at 2 09 22 PM (2)](https://github.com/dhanyakumarg/vvssdd/assets/132377400/9dc7fe39-e858-4a91-980a-cdb71368a6e6)
<br />
<br />
<br />

```bash
  $  write_verilog good_mux_netlist.v
 $  !gvim good_mux_netlist.v
```

![WhatsApp Image 2024-03-21 at 2 09 22 PM (3)](https://github.com/dha![WhatsApp Image 2024-03-21 at 2 09 22 PM (4)](https://github.com/dhanyakumarg/vvssdd/assets/132377400/c2c5113e-254b-4721-b725-873b5819670e)
nyakumarg/vvssdd/assets/132377400/6f50a5e7-08b4-40ff-b53b-5fcc2a6d8ca6)
```bash
  $  write_verilog -noattr good_mux_netlist.v
  $  !gvim good_mux_netlist.v
```
![WhatsApp Image 2024-03-21 at 2 09 22 PM (5)](https://github.com/dhanyakumarg/vvssdd/assets/132377400/e0231db6-3c14-4f79-85e6-637171587371)


## GTKWave

```bash
  $  iverilog iiit_pipo.v iiit_pipo_tb.v 
  $  ./a.out
  $  gtkwave tb_out.vcd
```
<br />
<br />

<br />


<br />

<br />

![WhatsApp Image 2024-03-21 at 2 09 22 PM (6)](https://github.com/dhanyakumarg/vvssdd/assets/132377400/05e7a066-008f-409b-8401-74158458cc6c)
