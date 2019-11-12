# korean-calendar
- MongoDB BSON data of Konrea calendar
- 2000y ~ 2100y Korean calendar with Solar calendar, Lunar calendar, Day of week and Holiday

## Detail
1. BSON keys (Column)
- sc : <string> Solar calendar 양력
- lc : <string> Lunar calendar 음력
- w : <int> Day of week 요일 (1 : Sun, 2 : Mon, 3 : Tue, 4 : Wed, 5 : Thu, 6 : Fri, 7 : Sat)
- h : <bool> Holiday 휴일
- ht : <string> Holiday detail 휴일 내용

## Usage
- Insert bson data to MongoDB Collection
```
mongorestore -h 127.0.0.1:27017 -d custom -c custom ./korean-calendar.bson
```
