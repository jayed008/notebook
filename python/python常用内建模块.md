1. time

   ```python
   >>> now = time.time()  # 当前时间 float类型
   >>> time.strftime("%Y-%m-%d %H:%M:%S")  #当前时间 str
   '2016-11-04 15:29:58'
   
   >>> time.ctime()   # 当前时间 english str
   'Fri Nov 4 15:40:42 2016'
   
   >>> time.time()
   1478244363.875308
   >>> time.localtime()   # 当前时间 time结构体
   time.struct_time(tm_year=2016, tm_mon=11, tm_mday=4, tm_hour=15, tm_min=26, tm_sec=9, tm_wday=4, tm_yday=309, tm_isdst=0)
   
   >>> time.localtime(now)  # float -> struct_time
   time.struct_time(tm_year=2016, tm_mon=11, tm_mday=4, tm_hour=15, tm_min=26, tm_sec=1, tm_wday=4, tm_yday=309, tm_isdst=0)
   
   >>> time.strftime('%Z', time.localtime())   # 显示当前时区 China standard timezone
   'CST'
   >>> time.gmtime()    # 显示UTC标准时间 跟中国相差8个钟
   time.struct_time(tm_year=2016, tm_mon=11, tm_mday=4, tm_hour=7, tm_min=26, tm_sec=28, tm_wday=4, tm_yday=309, tm_isdst=0)
   
   >>> a = '2016-11-04 15:29:58'  #时间字符串转化为time结构体
   >>> time.strptime(a, "%Y-%m-%d %H:%M:%S")  
   time.struct_time(tm_year=2016, tm_mon=11, tm_mday=4, tm_hour=15, tm_min=29, tm_sec=58, tm_wday=4, tm_yday=309, tm_isdst=-1)
   
   >>> a = '2016-11-04 15:29:58'  #时间字符串转成float类型
   >>> time.mktime(time.strptime(a, "%Y-%m-%d %H:%M:%S"))
   1478244598.0
   
   >>> time_tuple = (2016, 11, 04, 13, 51, 18, 2, 317, 0) #time tuple格式转成字符串
   >>> time.strftime("%Y-%m-%d %H:%M:%S", time_tuple)    
   '2016-11-04 13:51:18'
   
   >>> a = 1478244598.0           #float类型转成时间字符串
   >>> b = time.localtime(a)
   >>> time.strftime("%Y-%m-%d %H:%M:%S", b)
   '2016-11-04 15:29:58'
   ```
   
   
