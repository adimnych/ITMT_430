## Case Study #1 
## Lessons Learned From Scaling Uber To 2000 Engineers, 1000 Services, And 8000 Git Repositories

![Uber](/images/uber.jpg)
      
### What market does that company serve? (What do they do?) And have they always served that market?

Uber is a ride-hailing application, which allows customers to order rides, both private and shared with a few taps on their mobile devices. 

As of April 2016, Uber's Market included 

<ul>
<li>Cities Worldwide: 400+</li>
<li>Counties Worldwide: 70</li>
<li>Employees: 6000+</li>
</ul>

### What Operating System(s) are used?

At a lower level, Uber engineers use pre-history :   PHP (outsourced)
	

### Why do you think those were used?

Uber's huge growth spurt has caused much concern for all of its engineers. They have decided to use Microservices to break up all these. With microservices came the good and the bad, but it was said that Uber ultimately needed a tradeoff. 

### What programming languages/frameworks are used?


<ul>
	<li>Dispatch : 		Originally Node.JS, now moving to Go</li>
	<li>Core Services:  Originally Python, now moving to Go</li>
	<li>Maps:	 		Python and Java</li>
	<li>Data :			Python and Java</li>
	<li>Metrics : 		Go</li>
</ul>

### Why do you think they were used?

Microservices allowed team to be formed quickly to run independently. 

### What storage and what database technologies are used?

Uber's business runs on a hybrid cloud model, using many different providers and active data centers. Uber does not have a "backup system". 
One technology that Uber uses is Terraform, which is owned by HashiCorp. It defines infrastructure as code to increase operator
productivity. 
	

### What is the current stock price and what was the IPO of the company? (if traded publicly.)

Uber is on track for IPO in 2019. It's estimated market valuation is around $62 billion dollars. 
In which it plans to sell between $400-$600 million in stock at around $40 per share. 


### What major obstacle (cost, system performance, QPS, etc, etc) was the company trying to overcome by implementing this technology stack?

Uber also had performances issues, since RPC's were expensive. Understanding one language is easy, but
understanding performance across all the language is what made it a challenge. 
To overcome Fanout issues, Uber has used tracing. Uber used OpenTracing and Zipkin.

### What can you learn from this article relating to technology architecture?

I have learned that Uber had to make a lot of tradeoffs. Designing decisions that would help scale super high traffic needs.
Deciding to reduce Uber total of engineers to 2000, and services to 1,000 and git repositories to 8,000, many lessons were learned.
Learning how to use less services and repositiories using microservices had paved the future for Uber. After reading this article, I can 
see how microservice architecture, runs its own unique process, and manages its own database. By using microservices, Uber is able to 
reduce any failing components, and improve overall availability of its application

## Case Study #2 
## Netflix: What happens when you press play?
![Uber](/images/netflix.jpg)

### What market does that company serve? (What do they do?) And have they always served that market?

Netflix is a media-service provider. Now, they are subscription based. Originally, Netflix used to rent DVD's, but they moved towards 
cloud computing. Netflix allows its users to watch TV shows, movies and documentaries. The best part about Netflix is the flexibility 
for the users to watch anywhere, anytime on almost any device. 

Netflix Statistics for 2017:
<ul>
	<li> Netflix has more than 110 million subscribers. </li>
	<li> Netflix operates in more than 200 countries. </li>
	<li> Netflix has nearly $3 billion in revenue per quarter.</li>
	<li> Netflix adds more than 5 million new subscribers per quarter.</li>
</ul>

### What Operating System(s) are used?

Netflix's servers run on mostly open-source software - the FreeBSD operating system, as well as
nginx Web server. For routing, it uses BIRD software. 

### Why do you think those were used?
Netflix uses FreeBSD because of its stability, security and leighter weight. 
FreeBSD developers can manage the essntial operating systems remotely and effectively.
FreeBSD helps Netflix deliver all those hours of videos to all of its subscribers.

### What programming languages/frameworks are used?

Front-end: JavaScript
Backend: Java and Python
Frameworks: Node.js
Except from Node.js, netflix engineers use React and RxJS with the goal to vuild variable client applications that are suitable for 
different devices. 

### Why do you think they were used?

Netflix originally used Java on the server and javascript on the client, which had created many difficulties since the developers had to switch between both languages, and write eveything twice, two ways for accessing data and rendering.

### What storage and what database technologies are used?

The databases used at Netflix were MySQL, PostgreSQL, Cassandra, Oracle.
Netflix used to run two of their own data centers, and they have experienced many problems in the past.
Ultimately, Netfix move to Amazon Web Services (AWS). Netflix wanted to remove any and all single points of failure by using AWS 
reliable databases. Amazon EC2 was used as cloud hosting for infrastructure of Netflix, and Amazon S3 as cloud storage.
Currently

### What is the current stock price and what was the IPO of the company? (if traded publicly.)

The current stock price of Netflix, Inc is $328.90
The share price at IPO: $15.00 back in May 23,2002.
Valuation at IPO: $309.7 Million

### What major obstacle (cost, system performance, QPS, etc, etc) was the company trying to overcome by implementing this technology stack?
In 2008, Netflix had a major database corruption, which prevented Netflix from shipping DVD's to its customers. The major obstacle that 
Netflix had to overcome was going from Datacenters and DVD rentals to the cloud. By moving all of its operations to AWS, it was able to 
operate tens of thousands of servers and tens of petabytes of storage in the Amazon cloud. The amount of money Netflix has payed Amazon 
is unknown. Netflix did mention it had spend $800 million on technology and development in 2016, and will spend $7 billion dollars on 
new content in 2018.

### What can you learn from this article relating to technology architecture?

Netflix has saved lots of money using AWS. It is a data-driven company, and it uses its popularity data to predict which videos members 
will want to watch tomorrow in each location. After reading this article, I can see how "going to the cloud" can help any huge company 
save millions of dollars, instead of having their own datacenters. Netflix has a huge library of content, and using AWS allows Netflix 
to prepopulate the servers with content it thinks people will want to watch, reducing bandwith use in peak hours.
