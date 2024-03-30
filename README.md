# LCD pinout
LCD segments are either :
- Driven one by one in conjunction with a unique common pin.
- Multiplexed with several common pins if there are not enough pins with segments which is our case here.

There are 13 total pins, among which 9 are control pins the remaining 4 are common pins, in this order.

By probing the different pins with an oscilloscope, we can indeed comfirm the presense of two groups with the shape of the different waveforms.

Here is the determined pinout :

### Segment pins
1.  unit segments
2.  num 4, second segment
3.  num 4, first segment
4.  num 3, second segment
5.  num 3, first segment
6.  num 2, second segment
7.  num 2, first segment
8.  num 1, second segment
9.  num 1, first segment

### COM pins
10. COM d, dots, and f, e (num 0) segments
11. COM st, c, e
12. COM lb, b, g
13. COM kg, a, f


```
num 0         num 1           num 2           num 3           num 4
                                                           
              __a__           __a__           __a__           __a__             st 
|            |     |         |     |         |     |         |     |
f            f     b    .    f     b    .    f     b         f     b
|            |     |         |     |         |     |         |     |
              __g__           __g__           __g__           __g__             lb 
|            |     |         |     |         |     |         |     |
e            e     c    .    e     c    .    e     c         e     c
|            |     |         |     |         |     |         |     |
              __d__           __d__           __d__     .     __d__             kg

 ```
