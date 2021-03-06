# ipinfo
Return IP address info including geographic location and distance when given IP address, email address, host name or URL

IP geolocation is retrieved from https://ipinfo.io/

To install:

```
go get github.com/jftuga/ipinfo
```

Example:

```
macbook:ipinfo jftuga$ ./ipinfo amazon.com https://cisco.com user@github.com

+------------+-----------------+-----------------------------------------------+---------------------------+---------------+------------+---------+-------------------+----------+
|   INPUT    |       IP        |                   HOSTNAME                    |            ORG            |     CITY      |   REGION   | COUNTRY |        LOC        | DISTANCE |
+------------+-----------------+-----------------------------------------------+---------------------------+---------------+------------+---------+-------------------+----------+
| amazon.com | 176.32.98.166   |                                               | AS16509 Amazon.com, Inc.  | Ashburn       | Virginia   | US      | 39.0481,-77.4728  |   483.66 |
| amazon.com | 176.32.103.205  |                                               | AS16509 Amazon.com, Inc.  | Ashburn       | Virginia   | US      | 39.0481,-77.4728  |   483.66 |
| amazon.com | 205.251.242.103 | s3-console-us-standard.console.aws.amazon.com | AS16509 Amazon.com, Inc.  | Ashburn       | Virginia   | US      | 39.0481,-77.4728  |   483.66 |
| cisco.com  | 72.163.4.185    | redirect-ns.cisco.com                         | AS109 Cisco Systems, Inc. | Richardson    | Texas      | US      | 32.9462,-96.7058  |   769.31 |
| github.com | 192.30.253.113  | lb-192-30-253-113-iad.github.com              | AS36459 GitHub, Inc.      | San Francisco | California | US      | 37.7697,-122.3930 |  2186.72 |
| github.com | 192.30.253.112  | lb-192-30-253-112-iad.github.com              | AS36459 GitHub, Inc.      | San Francisco | California | US      | 37.7697,-122.3930 |  2186.72 |
+------------+-----------------+-----------------------------------------------+---------------------------+---------------+------------+---------+-------------------+----------+


your IP addr : w.x.y.z
your location: A,B
elapsed time : 450.60ms
```

Code discussion: https://old.reddit.com/r/golang/comments/9xd3a3/i_just_finished_my_first_go_program_ipinfo/

