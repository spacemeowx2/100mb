# 100mb
a 100mb file, 0x00, 0x01, 0x02....0xfe, 0xff, 0x00, 0x01....

```python
s=''.join([chr(i & 0xFF) for i in xrange(1024*1024*100)])
open('100mb.bin', 'wb').write(s)
```
