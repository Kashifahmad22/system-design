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