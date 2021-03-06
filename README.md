## Question 1: Design Facebook News Feed

In the Design Facebook News Feed question, design the following key features and their APIs.

Facebook users should see the news feed containing posts and statuses from their friends and pages that they have
followed. They can post and like statuses that may contain text, images, and videos. They can send friend requests to
other users and follow other pages.

### References

1. codeKarle[Video] [Facebook System Design | Instagram System Design | System Design Interview Question](https://www.youtube.com/watch?v=9-hjBGxuiEs)
2. SDE Skill[Video] [System Design Mock Interview - Facebook News Feed](https://www.youtube.com/watch?v=a7p0bVqYNZ8)

## Question 2: Design Live Commenting

This question is not related to Live Videos. This question is related to the active real-time feed of comments at the
bottom of each post. Thus, in this question,

Design the backend of a system that can enable real-time commenting on Facebook posts. The users should be able to see
the new comments in real-time for the posts visible in front of their screen. This problem is quite challenging, as
users are continuously scrolling the news feed, and thus the posts that are visible in their view can change very
frequently.

## Scale Estimations

To design an efficient system in the interview, we will have to consider the following scale estimations. These
estimations will help us in explaining the scale of the system to the interviewer.

Every minute, Facebook serves over 100 million pieces of content that may receive comments. In that same minute, users
submit around a million comments that need to get routed to the correct viewers.

### References

1. https://www.infoq.com/presentations/linkedin-play-akka-distributed-systems/

## Question 3: Design Facebook Messenger or WhatsApp

Develop the backend of a messenger system that can,

Support 1:1 conversations between two users. Track the online or offline status of the users. If time remains, discuss
more complex features like Group conversations and Push notifications.

### References

1. Tushar Roy [System Design : Design messaging/chat service like Facebook Messenger or Whatsapp](https://www.youtube.com/watch?v=zKPNUMkwOJE)
2. CodeKarle [WhatsApp System Design | FB Messenger System Design | System Design Interview Question](https://www.youtube.com/watch?v=RjQjbJ2UJDg)

3. Exponent[Video] [System Design Mock Interview: Design Facebook Messenger](https://www.youtube.com/watch?v=uzeJb7ZjoQ4)

## Question 4: Design Instagram

Design a simpler version of Instagram.

Users can upload and share photos. They can follow other users. Like the photos posted on Instagram. Instagram users
should get a scrollable feed of photos that are posted by the users they follow.

### References

1. https://www.youtube.com/watch?v=QmX2NPkJTKg

## Question 5: Twitter System Design

1. codeKarle [Twitter System Design | System Design Interview Question](https://www.youtube.com/watch?v=EkudBdvbDhs)

## Question 6: Distributed Logging Architecture

1. Blog [Distributed Logging Architecture in the Container Era](https://blog.treasuredata.com/blog/2016/08/03/distributed-logging-architecture-in-the-container-era/)
2. Twitter Blog [Building DistributedLog: High-performance replicated log service](https://blog.twitter.com/engineering/en_us/topics/infrastructure/2015/building-distributedlog-twitter-s-high-performance-replicated-log-servic.html)
3. Hackerkanoon [Building a Centralized Logging Application](https://hackernoon.com/part-1-building-a-centralized-logging-application-5a537033da0a)

## Question 7: Distributed Message Queue

References:

1. [System Design Interview - Distributed Message Queue](https://www.youtube.com/watch?v=iJLL-KPqBpM&t=1078s)
2. [Scaling Push Messaging for Millions of Devices @Netflix](https://www.youtube.com/watch?v=6w6E_B55p0E)

## Question 8: Distributed Cache

References:

1. [System Design Interview - Distributed Cache](https://www.youtube.com/watch?v=iuqZvajTOyA)
2. [https://www.youtube.com/watch?v=jzPSuBiidF4](https://www.youtube.com/watch?v=jzPSuBiidF4)

## Question 9: Rate Limiting (local and distributed)

References:

1. [Rate Limiting (local and distributed)](https://www.youtube.com/watch?v=FU4WlwfS3G0)

## Question 10: Top K Problem (Heavy Hitters)

References:

1. [System Design Interview - Top K Problem (Heavy Hitters)](https://www.youtube.com/watch?v=kx-XDoPjoHw&t=948s)

## Question 11: Notification Service

References:

1. [System Design Interview - Notification Service](https://www.youtube.com/watch?v=bBTPZ9NdSk8)
2. [Notification Service System Design Interview Question to handle Billions of users & Notifications](https://www.youtube.com/watch?v=CUwt9_l0DOg)
3. [Real-Time & Personalized Notifications @Twitter](https://www.youtube.com/watch?v=pme_n2zQiDQ)

## Question 12: Design Typeahead Suggestions

Google predicts and suggests a list of autocomplete queries based on the characters that we have already typed in the
search box.

Suggest the top ten search queries based on the characters already typed by the user in the search box. Assume query's
popularity can be determined by the frequency of the query being searched in the past.

1. Tushar Roy [System design : Design Autocomplete or Typeahead Suggestions for Google search](https://www.youtube.com/watch?v=us0qySiUsGU)

## Question 13: Design Proximity Server(Yelp/Nearbuy)

Proximity servers are used to discover nearby attractions such as places and events, which are then recommended to
Facebook users.

Users can add, update, and delete places. Given a location expressed as latitude and longitude, users can query all the
nearby places within a given distance. Optional Follow-up: Query events near a given place around a particular time.
This adds the third dimension of time to the problem.

1. [Yelp system design | amazon interview question Yelp software architecture](https://www.youtube.com/watch?v=TCP5iPy8xqo)

## Question 14: Design Web Crawler

Web Crawler scans the world wide web to download and index all the web pages to be made available for the search queries
submitted by the users.

Given a list of seed web pages, it should download all the web pages and index them for future retrieval. The service
should handle duplicate web pages so that unique URLs are stored.

### Design Goals

1. We should ensure that our service is highly scalable, as it needs to crawl the entire Web and fetch billions of web
   pages.
2. It should implement the Robot Exclusion protocol, allowing web admins to declare parts of their websites off-limits
   to crawlers.
3. For the simplicity of the interview, we can consider that we will crawl only HTML pages.

References:

1. Tech Dummies Narendra L[Video] [System Design distributed web crawler to crawl Billions of web pages | web crawler system design](https://www.youtube.com/watch?v=BKZxZwUgL3Y)
2. Justin Barnett [Video] [System Design Interview: Design a Web Crawler](https://www.youtube.com/watch?v=l9z5_YSIZyM)

### Scale Estimations

1. Our System will be crawling about 25 billion web pages every two weeks.
2. On average, each URL will be 512 bytes in size,
3. And each page will be about 100 KB in size.

## Question 15: BOOKMYSHOW System Design

References:

1. Tech Dummies Narendra L[Video] [BOOKMYSHOW System Design, FANDANGO System Design | Software architecture for online ticket booking](https://www.youtube.com/watch?v=lBAwJgoO3Ek)

## Question 16: URL Shortening

1. Narendra L [URL shortener system design | tinyurl system design | bitly system design](https://www.youtube.com/watch?v=JQDHz72OA3c&list=PLkQkbY7JNJuC99VDJcpQdww-4aT3QhdJv&index=21)

## Question 17: Stock exchange

1. Narendra L [STOCK EXCHANGE SYSTEM DESIGN | AMAZON INTERVIEW QUESTION DESIGN STOCK EXCHANGE](https://www.youtube.com/watch?v=dUMWMZmMsVE)

## Question 18: Pastebin

Pastebin allows you to paste text or code and then share a link to that code anywhere you want. It???s not an online code
editor but you can use this to store any kind of text.

1. Narendra L [Paste bin system design | Software architecture for paste bin](https://www.youtube.com/watch?v=josjRSBqEBI)

## Question 19: Google Drive or Dropbox

These are used to store and share files, photos, and other media. How do you go about designing things like allowing
users to upload/view/search/share files or photos? track permissions for file sharing, and allow multiple users to edit
the same document?

1. [Dropbox system design | Google drive system design | System design file share and upload](https://www.youtube.com/watch?v=U0xTu6E2CT8)

## Question 20: Ride-hailing service e.g. Uber, or Ola

1. codeKarle[Video] [Uber System Design | Ola System Design](https://www.youtube.com/watch?v=Tp8kpMe-ZKw)

## Question 21: Airbnb

1. codeKarle[Video] [Airbnb System Design | Booking.com System Design | System Design Interview Question](https://www.youtube.com/watch?v=YyOXt2MEkv4)

## Question 22: Amazon or Flipcart

1. CodeKarle [Amazon System Design | Flipkart System Design](https://www.youtube.com/watch?v=EpASu_1dUdE)

## Question 23: Parking Lot system

1. [System Design Interview Question: DESIGN A PARKING LOT - asked at Google, Facebook](https://www.youtube.com/watch?v=DSGsa0pu8-k)

## Question 24: Design Netflix/Youtube

1. codeKarle[Video] [Netflix System Design | YouTube System Design ](https://www.youtube.com/watch?v=lYoSd2WCJTo)
2. Narendra
   L[Video] [NETFLIX System design | software architecture for netflix](https://www.youtube.com/watch?v=psQzyFfsUGU)

## Question 25: Zoom System Design | WhatsApp / FB Video Calling System Design

1. codeKarle[Video] [Zoom System Design | WhatsApp / FB Video Calling System Design | System Design Interview Question](https://www.youtube.com/watch?v=G32ThJakeHk)

## Question 26: Google Maps System Design

1. codeKarle[Video] [Google Maps System Design Interview Question](https://www.youtube.com/watch?v=jk3yvVfNvds)