
# 时间戳转换
```python
import time
def timeex(tq):
    if len(str(tq))==13:
        ts = int(tq)/1000
    elif len(str(tq))==10:
        ts =int(tq)
    putime=time.localtime(ts)
    print(putime)
    otherStyleTime = time.strftime("%Y-%m-%d", putime)
    print(otherStyleTime)
    return otherStyleTime
                                   
if __name__ == '__main__':
    
    t= '1539939436000'
    timeex(1539939436)

        
```
