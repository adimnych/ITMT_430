## Case Study #1 
## Lessons Learned From Scaling Uber To 2000 Engineers, 1000 Services, And 8000 Git Repositories

![Uber](/images/uber.jpg)

## Question and Answers:
      
### What market does that company serve? (What do they do?) And have they always served that market?


Uber is a ride-hailing application, which allows customers to order rides, both private and shared with a few taps on their mobile devices. 

As of April 2016, Uber's Market included 

Cities Worldwide: 400+
Counties Worldwide: 70
Employees: 6000+


### What Operating System(s) are used?

At a lower level, Uber engineers use pre-history :   PHP (outsourced)
	

### Why do you think those were used?

Uber's huge growth spurt has caused much concern for all of its engineers. They have decided to use Microservices to break up all these. With microservices came the good and the bad, but it was said that Uber ultimately needed a tradeoff. 


### What programming languages/frameworks are used?

Dispatch : 		Originally Node.JS, now moving to Go
Core Services:  	Originally Python, now moving to Go
Maps:	 		Python and Java
Data :			Python and Java
Metrics : 		Go


### Why do you think they were used?

Microservices allowed team to be formed quickly to run independently. 

### What storage and what database technologies are used?

Uber's business runs on a hybrid cloud model, using many different providers and active data centers. Uber does not have a "backup system". 

One technology that Uber uses is Terraform, which is owned by HashiCorp. It defines infrastructure as code to increase operator productivity. 
	

### What is the current stock price and what was the IPO of the company? (if traded publicly.)

	Uber is on track for IPO in 2019. It's estimated market valuation is around $62 billion dollars. 
	In which it plans to sell between $400-$600 million in stock at around $40 per share. 


### What major obstacle (cost, system performance, QPS, etc, etc) was the company trying to overcome by implementing this technology stack?

Uber also had performances issues, since RPC's were expensive. Understanding one language is easy, but
understanding performance across all the language is what made it a challenge. 
To overcome Fanout issues, Uber has used tracing. Uber used OpenTracing and Zipkin.

### What can you learn from this article relating to technology architecture?

	I have learned that Uber had to make a lot of tradeoffs. Designing decisions that would help scale super high traffic needs.
	Deciding to reduce Uber total of engineers to 2000, and services to 1,000 and git repositories to 8,000, many lessons were learned. Learning how to use less services and repositiories using microservices had paved the future for Uber.



## Case Study #2 
## Netflix: What happens when you press play?
![Uber](/images/netflix.jpg)
## Question and Answers:

### What market does that company serve? (What do they do?) And have they always served that market?

Netflix is a media-service provider. They are subscription based. 



### What Operating System(s) are used?

### Why do you think those were used?


### What programming languages/frameworks are used?

### Why do you think they were used?


### What storage and what database technologies are used?


### What is the current stock price and what was the IPO of the company? (if traded publicly.)


### What major obstacle (cost, system performance, QPS, etc, etc) was the company trying to overcome by implementing this technology stack?


### What can you learn from this article relating to technology architecture?


