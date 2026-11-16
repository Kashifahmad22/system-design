THis is system design notes:
Begore Designing anything always ask these questions:-
1.How many users and How fastly the user base is increasing 
2.Read Heavy or write heavy
3.What can you never Loose 
4.how much latency can you afford 
5.what does it cost 

If the intervier asks design an an app 
the candidate must ask followup questions like :
1. who is this for (user base) and the e3xact no. of users 
2.Is the app ready heavy or write heavy
3.The data should Never lost
4.speed is the primary objective 

types of systems/architecture:
1.monolith 
One codebase , one deploy
one running thing 
each function call each other 

2. Microservices
1.split onto many programs 
2.each program is deployed separately over their separate server 
3.independant scaling 
4.the system divided into teams the team can work separately without disturbing each other's work.

#Types of scaling 
1. Vertical Scaling 
adding more powerful device , when added can't be configued and also the prices don't increase in st. line so when the prices increase , moving to horizontal scaling is difficult.
2. Horizontal Scaling 
adding more number of servers , wehn added each server has the copy of the application and can run independantly and can reduce the load and is preffered for scaling applications and balancing the load.
2.any number of servers can be added whenever required.

#What is a Load balancer 
1.It's just a server running an application and it's primary use is to receive the request and send to one of the server.
2.It's the type of reverse proxy 
3.How does the load balancer stops itself , sending a reques to a dead server. 
It constantly does the health check of each of the server so that It get's the idea of dead server before sending the rquest.

#How does a load balancer picks a server?
1.It keeps the count of no. of pending rquests of each server,picks the server with least no. of server request pending.
2.Keeps counts internally.
3.It also does weighted distribution .

#what if the  load balancer fails itself
this is the reason why companies have multiple load balancers , so if one fails they can distribute the traffic to other load balancer.