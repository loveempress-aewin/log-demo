```log ================================================================
[root@localhost v1.01]#   date
Wed Sep 30 15:51:26 CST 2026
[root@localhost v1.01]#  ./psu -r
PSU0 Status   : RUN
PSU0 Vin      : 76.380 Volts
PSU0 +12V     : 25.500 Volts
PSU0 Fan      : 1900 RPM
PSU0 Temp.    : 25 degrees C
PSU0 Pin      : 82.320 Watts
PSU0 Pout     : 98.000 Watts
PSU0 POut_Max : N/A

PSU1 : Module has been removed or the device has failed.

[root@localhost v1.01]#  date
Wed Sep 30 15:52:13 CST 2026
[root@localhost v1.01]#  ./psu -r
PSU0 Status   : RUN
PSU0 Vin      : 112.560 Volts
PSU0 +12V     : 25.500 Volts
PSU0 Fan      : 4400 RPM
PSU0 Temp.    : 19 degrees C
PSU0 Pin      : N/A
PSU0 Pout     : 98.000 Watts
PSU0 POut_Max : N/A

PSU1 Status   : RUN
PSU1 Vin      : 112.560 Volts
PSU1 +12V     : 15.100 Volts
PSU1 Fan      : N/A
PSU1 Temp.    : N/A
PSU1 Pin      : 117.600 Watts
PSU1 Pout     : 101.920 Watts
PSU1 POut_Max : N/A

[root@localhost v1.01]#
```
看到上面的兩次結果 我都沒有動我的硬體 但是他的數值亂檢測
可以發現他自己沒偵測到PSU1

### 3 ~ 6 time

```log ================================================================
[root@localhost v1.01]#  date
Wed Sep 30 15:53:05 CST 2026
[root@localhost v1.01]#  ./psu -r
PSU0 Status   : RUN
PSU0 Vin      : 112.560 Volts
PSU0 +12V     : 25.500 Volts
PSU0 Fan      : 600 RPM
PSU0 Temp.    : N/A
PSU0 Pin      : 82.320 Watts
PSU0 Pout     : 98.000 Watts
PSU0 POut_Max : N/A

PSU1 Status   : RUN
PSU1 Vin      : 112.560 Volts
PSU1 +12V     : 25.500 Volts
PSU1 Fan      : 2200 RPM
PSU1 Temp.    : 25 degrees C
PSU1 Pin      : 117.600 Watts
PSU1 Pout     : 78.400 Watts
PSU1 POut_Max : N/A

[root@localhost v1.01]#  PSU #### 5
Wed Sep 30 15:54:37 CST 2026
PSU0 Status   : RUN
PSU0 Vin      : 112.560 Volts
PSU0 +12V     : 16.900 Volts
PSU0 Fan      : 1800 RPM
PSU0 Temp.    : N/A
PSU0 Pin      : 109.760 Watts
PSU0 Pout     : 98.000 Watts
PSU0 POut_Max : N/A

PSU1 Status   : RUN
PSU1 Vin      : 112.560 Volts
PSU1 +12V     : 23.500 Volts
PSU1 Fan      : 2200 RPM
PSU1 Temp.    : 19 degrees C
PSU1 Pin      : 86.240 Watts
PSU1 Pout     : 101.920 Watts
PSU1 POut_Max : N/A

[root@localhost v1.01]#  PSU #### 6
Wed Sep 30 15:54:56 CST 2026
PSU0 Status   : RUN
PSU0 Vin      : 112.560 Volts
PSU0 +12V     : 13.800 Volts
PSU0 Fan      : 800 RPM
PSU0 Temp.    : N/A
PSU0 Pin      : 82.320 Watts
PSU0 Pout     : 98.000 Watts
PSU0 POut_Max : N/A

PSU1 Status   : RUN
PSU1 Vin      : 112.560 Volts
PSU1 +12V     : 14.400 Volts
PSU1 Fan      : N/A
PSU1 Temp.    : 6 degrees C
PSU1 Pin      : 117.600 Watts
PSU1 Pout     : 101.920 Watts
PSU1 POut_Max : N/A
```
