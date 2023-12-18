# Snail-loris 

  The low bandwidth, yet greedy and poisonous HTTP client


  Snail-loris is simple Slowloris HTTP DoS attack tool, destroyer of the cyber worlds


  Slowloris is a simple, dangerous and elegant denial of service attack that uses low bandwidth
  to take down a machine's web server with a single machine

  It affects threaded servers

  Slowloris was first invented by "Robert "RSnake" Hansen" an american computer hacker

  
  Slowloris establishes many simultaneous connections to the victim server and holds these open for as long as possible by very slowly sending HTTP headers
  but nevercompleting the requests by sending half finished request or partial request


  This keeps the server busy waiting for the rest of the data, and if the maximum current connection pool is filled, 
  actual clients attempting to connect to the server will fail


  Slowloris is not a TCP DoS because it is actually making a full TCP connection, 
  not a partial one, however it is making partial HTTP requests. 
  it's the equivalent of a SYN flood but 
  over HTTP......


  Slowloris exploit most threaded site running on

  Apache 1.x
   
  Apache 2.x
    
  dhttpd
   
  GoAhead WebServer
    
  WebSense 
   
  Trapeze Wireless Web Portal 
   
  Verizon's MI424-WR FIOS Cable modem 

  BeeWare
   
  Deny All
   
  Flask development server and so on.....



  Slowloris only represents one variant an DOS attack



# Command


 git clone https://github.com/Gbolahanomotosho/Snail-loris 




 cd Snail-loris 



 pip install -r requirements.txt




 python Snail-loris.py





# tested on :


- Linux


- Termux(Not yet tested though)


# NB: 

 Dont run on window machine 

 Since windows appears to limit how many sockets you can have open at any given time

 Slowloris works way better if run from a *Nix box than from Windows and not from within a virtual machine

 It has to do with the fact that Windows limits the amount of open sockets you can have at once to a fairly small number....

 Slowloris requires more than a few hundred sockets to work (sometimes a thousand or more), and Windows limits sockets to around like 130
 

# Disclaimer:

 For educational purpose only

 Use responsibly and do not point the tool at servers that you do not own/control. 

 It's illegal and you are liable for damage caused.

 It is advisable to use on your own personal server......


#Updated version:

 SSL and Tor mask ip will be added at the next updated version

 Happy Slowloris..... 
