convert.js
=====
This is a simple conversion library

convert.metric(data, source, target)
-----------------------

```javascript
convert.metric(1, "cm", "m");
=> 0.01

convert.metric(1, "hm", "inch");
=> 3937.0078740157

convert.metric(1, "km", "mm");
=> 1000000

convert.metric("string", "dam", "yard");
=> false
```

convert.DataUnits(data, source, target)
-----------------------

```javascript
convert.DataUnits(1, "mb", "kb");
=> 1024

convert.DataUnits(1, "byte", "tb");
=> 9.0949470177293e-13

convert.DataUnits("string", "gb", "pb");
=> false
```

convert.Temperature(data, source, target)
-----------------------

```javascript
convert.Temperature(1, "c", "k");
=> 274.15

convert.Temperature(1, "n", "c");
=> 3.0303030303030303

convert.Temperature(1, "f", "n");
=> -5.68323

convert.Temperature("string", "k", "f");
=> false
```

convert.Time(data, source, target)
-----------------------

```javascript
convert.Time(1, "second", "millisecond");
=> 1000

convert.Time(1, "hour", "minute");
=> 60

convert.Time(1, "week", "year");
=> 0.019164955509925

convert.Time("string", "day", "century");
=> false
```