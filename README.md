Hello , 
This repository is help to verify the synchronous FIFO using system verilog. The project is very basic and done with some help of Udemy course by Kumar Khandagle. so to verify the FIFO functionality we define different classes : 
1. Transaction class :  To define the variables
2. Generator class : Generate random stimulis
3. Driver class : recieve the variable from Generator class through mailbox and send them to interface
4. Monitor class : take element from interface and send them to scoreboard using mailbox
5. Scoreboard class : Take elemenet from monitor and verify them with golden data .

   This is the basic structure of classes we defined here .

   So in the first class transaction class we define some variable  and define one variable operation which we are generation random values it is one bit so it define whcih operation FIFO is using read and write if read menad operation value is 0 and write means operation value is 1 .
   Second class is generator class we are generating random value of oper variable and sending them to driver.
   third class is driver we defined three task first is reset where ew take for first 5 clock reset high and after that reset is low in second task we write the data in memory.
   in third task we define reading where rd is high and other wr and rst is zero .
   and there is also one task which run all threse three task and getting data from generator

   next class is monitor we getting data form the interface and supply the data to scoreboard .
   socreaboard verifies the data with the golden data .
