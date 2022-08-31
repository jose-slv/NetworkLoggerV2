# NetworkLoggerV2
****

>New tool to generate TCP traffic and packet capture according to your needs.

--------

### Simple tutorial on how to work with NetworkLogger.

#### The folder will have the following files:
![Screenshot_2](https://user-images.githubusercontent.com/110167869/187642875-d44ca28a-4ee5-44ef-9f92-19f003eb64f8.png)



#### We can then open the highlighted “NetworkLogger.exe” file that would lead us to the following window:

 ![image](https://user-images.githubusercontent.com/110167869/182665122-fc5973e7-1816-49d1-a207-36baa904f197.png)

```
1 - Text box to insert the test string.
2 - Button to leave the program.
3 - Button to start the program.
4 - Information on the string Syntax.
```

#### Now we can insert the string following the syntax:

```
Generate TCP traffic and Packet Capture:  "<DestinationIP>,<TCPport>,<Normal/Circular>" Ex: 1.1.1.1,80,normal
Simply packet capture: "**"
````

### A packet capture choice of either Normal or Circular would lead us to the next window:

 ![image](https://user-images.githubusercontent.com/110167869/182665288-6b4fbc5a-80b0-4626-aad2-f5676179a120.png)

```
1 - TCP Statistics
2 - Packet Capture details
3 - Txt file information
4 - Path of created files
5 - TCP output 
6 - Revert to initial window
7 - Redo the tests
8 - Close the Application
  ``` 
>Throughout the process we have various messages, showing what's being written on the CMD and the output of the same. Making the application as transparant as possible to the end user.

##### Initial Pop up with pktmon command inserted on the CMD.
![Screenshot_3](https://user-images.githubusercontent.com/110167869/187643702-56f936ca-ce22-40b4-b0ef-e4f5f9b9a866.png)


 
##### After concluding the TCP connections:
  
```
Normal : 10 TCP connections.
Circular: Loop until it finds an issue, if one connection fails, it will do 15 more TCP connections and conclude the proccess.
```
  
##### Pop up indicating pktmon capture stopped and files generated.
  
![Screenshot_4](https://user-images.githubusercontent.com/110167869/187643639-ac4492a1-4079-4bfb-b725-41047c12b8dd.png)


 
##### Pop up indicating file conversion from Etl to Pcapng.
  
![Screenshot_5](https://user-images.githubusercontent.com/110167869/187643522-f30f0a92-4520-4514-8af0-a4f69d8803be.png)



### After this, if you reach your output folder, you’ll be able to find the following:

![Screenshot_6](https://user-images.githubusercontent.com/110167869/187643860-b2c882bc-d72a-49d3-bb14-e14182487dff.png)

                                                                                                        
-------
  
## How to simply use the tool to packet capture on a windows device?
  
 >Simply use the string "**" on the first 
  
### The window you would see is as follows:
  
![image](https://user-images.githubusercontent.com/110167869/182667041-e1ab301c-8b44-46e4-bf77-69cb85261be7.png)

 
 ```                                                 
1 – State of the packet capture
2 – Files generated Location
3 – Button to stop the capture
  ``` 
  
****

## FAQ
#### What is the difference from the V1 to V2 of NetworkLogger?
>The V1 will use NETSH for the packet capture, while the V2 is using pktmon.

#### What is used to generate the packet captures?
> pktmon is used to packet capture via CMD.
 
#### Do i need to open the file in admin mode?
>Yes, otherwise it's not possible to run Netsh on the CMD.

 
