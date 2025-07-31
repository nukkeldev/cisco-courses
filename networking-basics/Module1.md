# Module 1: Communication in the Connected World - Notes

## Section 1: Network Types

> Apparently, Internet is short for Inter-network... though it makes sense since the Internet is
> just a bunch of interconnected networks.

### Local Networks

Networks come in various scales, but a common aspect is that they connect devices together,
possibly to other remote resources (i.e. network drives, corporate networks, etc.), and to the
internet. As they scale, networks could be comprised of sub-networks to form a "network of
networks".

Devices can come in a variety of forms: from laptops and desktops, to mobile devices, or to IoT
devices. Some devices may be designed to be connected to the internet, while others may be purely
local or specialized for another method of communication (i.e. RFID tags).

## Section 2: Data Transmission

> Data can be collected in many ways: volunteered by users (i.e. posts, comments, etc.), 
> inferred from activity (i.e. CC activity, posts, etc.), or observed (i.e. location services,
> etc.).

### Bits & Bytes

> I am taking notes on this for completeness take... I am well aware of these.

Bits are the "fundamental language of computers". They are binary in that they can only ever by
0 or 1, regardless of the method of storage (i.e. light intensities, voltages levels, etc.)  
Further, eight bits make up one byte. Practically, the American Standard Code for Information
Interchange (ASCII) is a common representation of encoding a limited subset of characters where
each character can be represented with a single byte.

### Data Transmission

Data is transmitted over _network media_. Common types of network media include copper wire,
fiber-optic cables, and electromagnetic waves. Combinations of these media are common in
practice to get the data to its destination. All forms of media are able to encode the data's
bits as two observably unique states. _Signals_ are transmitted across media in many forms, but 
in reference to the above media examples, three common methods are: electrical, optical, and
wireless signals. 

While electrical and wireless signals are found in networks of all scales, media using optical
signals are more prevalent in larger networks, as they can span larger distances while being 
significantly faster (and more expensive).

## Section 3: Bandwidth and Throughput

A network media's rate of data transfer is discussed in terms of _bandwidth_ and _throughput_.

### Bandwidth

Bandwidth is the _maximum_ capacity of a medium to carry data. Most often, bandwidth is measured
in the amount of _bits_ that can be sent across a medium per second. Common units include: 
- `b/s` - Bits per second (the base unit)
- `Kb/s` - (Kilobits) Thousands of `b/s`
- `Mb/s` - (Megabits) Millions of `b/s`
- `Gb/s` - (Gigabits) Billions of `b/s`
- `Tb/s` - (Terabits) Trillions of `b/s`
Measurements are influenced by physical properties of the medium and the laws of physics.

### Throughput

Throughput is the realized counterpart of a medium; how much the medium can actually achieve.
Alongside the influences of bandwidth, throughput is further influenced by the amount of data,
the type of data, and the latency of intermediary devices, just to name a few. _Latency_ refers
to the amount of time it takes for data to travel from one point to another. Throughput does not
care about validity of the data is focused purely on speed. A network's throughput is only as fast
as its slowest segment.

## Section 4: Summary

> Quiz Results: 11/11