---
title: Assignment 1
subtitle: Computer performance, reliability, and scalability calculation

author: Aritzi Piedras Silva

---


## 1.2 


#### a. Data Sizes

| Data Item                                  | Size per Item | 
|--------------------------------------------|--------------:|
| 128 character message.                     | 128 Bytes     |
| 1024x768 PNG image                         | 1 MB          |
| 1024x768 RAW image                         | 7.5 MB        | 
| HD (1080p) HEVC Video (15 minutes)         | 36 MB         |
| HD (1080p) Uncompressed Video (15 minutes) | 36000 MB      |
| 4K UHD HEVC Video (15 minutes)             | 228 MB        |
| 4k UHD Uncompressed Video (15 minutes)     | 228000 MB     |
| Human Genome (Uncompressed)                | 1.5 GB        |

1. 1 character is 8 bits ? so 128 character message is 128 bytes. 
2. Pixels 1024x768 = 786432 each pixel in an img needs 3 bytes in memory.
3. depth of 10  = 1024 * 768 * 1024 = 2.25mb png
4. 30 fps 8 bit depth x 15 mins= 900s *30*1290*1080*8/8/1000/1024 36 mb 
5. 1000 x 4 = 36k mb
6. 4k x 15 mins: 30*900*4096*2160*8/8/1000/1024/1023 = 228mb
7. 1000x larger = 228000mb 
8. 6*10^9 = genome x 1 byte/4 = 1.5 gb 


#### b. Scaling

|                                           | Size     | # HD | 
|-------------------------------------------|---------:|-----:|
| Daily Twitter Tweets (Uncompressed)       | 64 GB    | 1    |
| Daily Twitter Tweets (Snappy Compressed)  | 43 GB    | 1    |
| Daily Instagram Photos                    | 75 TB    |23    |
| Daily YouTube Videos                      | 104 TB   |32    |
| Yearly Twitter Tweets (Uncompressed)      | 23 TB    | 7    |
| Yearly Twitter Tweets (Snappy Compressed) | 15 TB    | 5    |
| Yearly Instagram Photos                   | 27375 TB | 8213 |
| Yearly YouTube Videos                     | 37960 TB |11388 |

1. 500 million tweets sent per day = 500 million * 128 bytes = 64 GB
2. 1.5 - 1.7x ratio plain txt if use 1.5 = 43 gb
3. .75 *100000000*1mb = 75000000mb = 75TB
4. 500 hrs *60*24 = 72k hrs * 60 mins = 720000 * 4 / 15 mins. 72k hrs * 4 * 36mb = 103680000mb 
5. 64gb *365 = 23360 = 23 tb 
6. 43 gb * 365= 23360 gb = 23 tb 
7. 75 tb *365 = 27375 = 15 tb 
8. 104 tb * 365 = 27375 tb 

#### c. Reliability
|                                    | # HD | # Failures |
|------------------------------------|-----:|-----------:|
| Twitter Tweets (Uncompressed)      |   7  |     <1     |
| Twitter Tweets (Snappy Compressed) |   5  |     <1     |
| Instagram Photos                   |8213  |     73     |
| YouTube Videos                     |11388 |     101    |


#### d. Latency

|                           | One Way Latency      |
|---------------------------|---------------------:|
| Los Angeles to Amsterdam  | 30 ms                |
| Low Earth Orbit Satellite | 40 ms                |
| Geostationary Satellite   | 600 ms               |
| Earth to the Moon         | 1281 ms              |
| Earth to Mars             | 3 minutes            | 

2. https://www.omniaccess.com/leo/#:~:text=The%20GEO%20latency%20is%20of,and%20an%20essential%20part%20if.


