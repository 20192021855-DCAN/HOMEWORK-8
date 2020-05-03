P9、    

Destination Address	Link Interface      
200.23.16/21	0          
200.23.24/24	1         
200.23.24/21	2         
otherwise	3          
P16、              

a) 家庭地址：192.168.1.1、192.168.1.2、192.168.1.3，      
路由器接口为192.168.1.4       

b)         

NAT Translation Table        	
WAN Side	LAN Side       
24.34.112.235, 4000	192.168.1.1, 3345    
24.34.112.235, 4001	192.168.1.1, 3346        
24.34.112.235, 4002	192.168.1.2, 3445         
24.34.112.235, 4003	192.168.1.2, 3446     
24.34.112.235, 4004	192.168.1.3, 3545        
24.34.112.235, 4005	192.168.1.3, 3546        
P20、            

S2 Flow Table	         
Match	Action         
Ingress Port = 3; IP Dst = 10.1..	Forward (2)             
Ingress Port = 3; IP Dst = 10.3..	Forward (2)         
Ingress Port = 4; IP Dst = 10.1..	Forward (1)       
Ingress Port = 4; IP Dst = 10.3..	Forward (1)            