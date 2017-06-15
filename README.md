# Milliseconds
A small python script to calculate the distance between two points on the earth in milliseconds.

## Motivation
Many problems in computer networking are dependent upon the travel time between two computer systems (c.f. *The 500 Mile Email*). If these systems are in different corners of the globe, this time may be relatively large. 

Beyond about 80 milliseconds of latency, interactive connections (i.e. phonecalls) become difficult to use.

This script helps the operator determine pure speed-of-light limits on how fast their data can move between two geographic points. It assumes a perfect, nap-of-the-earth route, and makes no accounting for actual fiber optic routes or delays caused by routers and network congestion.

## Usage
`./milliseconds "Los Angeles" "Sydney"`

returns:
> The direct distance between LA, Los Angeles County, California, United States of America and Sydney, NSW, Australia is 12061 kilometers. The fastest possible time between these points is 40 ms in a vacuum and 60 ms through optical fiber.

## Dependencies
[GeoPy](https://pypi.python.org/pypi/geopy)

## License
Copyright 2017. John Heenan

Released under the Mozilla Public License 2.0.

## To Do
    *   Add command line flags to return values, instead of the current verbose paragraph.
