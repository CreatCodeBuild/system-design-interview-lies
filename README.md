# system-design-interview-lies
Maybe system interview design questions &amp; answers are lies.

I am a professional software engineer with a Computer Science bachelor degree from a top university in US.  
I have 3.5 years professional experience working for Silicon Valley web & tech companies as the time of writting.   
I now work as a distributed system / infrastructure engineer in a database company.  
Though 90%+ of my work have been on the foundation of previous design and implementation. But I had the luck to design and implement some new system as well.

I have never passed a system design interview.

# URL Shortener
Last week, I was in a interview and the interviewer asked me to design a URL shortner. I gave a design.   
But apparently the interviewer did not think the design qualifies and I failed the interview.

2 years ago, I also had the same question in a different interview. I also failed that one.

2 consecutive failures of the same question kept me wondering. Is it true that I have to gave a template answer of URL shortner in order to pass the interview?  
Considering URL shortner a popular question, there are many best answers on the internet.   
Of course, I did not give those best answers, I gave answers according to my understanding of software engineering and compute science.

But still I felt super annoied by the fact that I failed these system design interviews. 

I want to implement 2 URL shortners. One with my naive design and another with the "best" template answer on the internet.

Maybe I will learn a lesson or 2. Or maybe those best template answers are lies.

## Requirement
The short URL has 5 chars. a-z and 0-9. Each char has 36 choices. That's a total of 36^5 = 60,466,176 (60 million) urls.
The minimal QPS of the service is 100,000. Let's say 25% are new URLs and 75% are reads of short URLs.

With this rate, the service will run out of short URLs in 40 minutes.

If the system can stand available in until ran out of short URLs, the system will pass. If both pass, the one with less overall (avg, mid, 99%, 95%) latency wins.

## Design A: My naive design

## Design B: Best Answer on the internet
