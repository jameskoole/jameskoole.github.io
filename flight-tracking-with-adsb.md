## Flight Tracking with ASD-B

A few months back, before the COVID-19 pandemic basically destroyed air traffic, I set up a Raspberry Pi as an ADS-B feeder for aircraft data in my area.

ADS-B stands for Automatic dependent surveillance–broadcast and it’s a technology that allows aircraft to transmit their positional data over open airwaves in order to be tracked by anyone who wishes to receive and decode it.

It’s meant to function as part of the Next-Generation Air Transportation System and forms the backbone of a new air traffic navigation system for the next century.

How it works isn’t really important, but the fact that anyone can set up a receiver, add some software to decode the data and display it on a map, is amazing. From there, you can feed the data to popular aggregators that allow anyone, anywhere in the world to see almost all the aircraft in the sky anywhere in the world in real time.

### My Setup
Receiving and feeding ADS-B requires both hardware and software. Everything is pretty easy to acquire and install, as long as you have some computer skills and the ability to follow instructions.

#### Hardware

I opted to purchase a few things from Amazon to get started. My total investment was about $150 for the hardware. The software is all open source and provided for free. Supplying data to various sites gets me premium accounts that offer some big benefits to aviation enthusiasts.

* Raspberry Pi 4 - this credit-card sized computer runs Linux and can be had for as little as about $40. I opted for a model with 4GB of RAM along with a case and power supply.
* FlightAware Pro Stick Plus SDR - a USB software defined radio receiver, specifically tuned to the ADS-B band with some special filters to improve reception of the signals from aircraft.
* FlightAware 1090MHz ADS-B Antenna - a tuned outdoor antenna that really improves range. In my case, I also added a 25ft. cable to run from the Raspberry Pi, through the wall and to my antenna which is mounted on our second-floor deck.

#### Software
On the software side, I used the FlightAware package for Raspberry Pi to get started with feeding. Once that was up and running, I layered the FlightRadar24 software on top and began feeding data to both services.

The FlightAware software has a built-in webserver that creates a local tracking site that shows all the aircraft being tracked by my system on a map with tracks and other details. They also have a stats page on the web that is publically accessible where you can see lots of details about my feeder including flights tracked over the last 30 days, range information and more.

Both FlightAware and Flightradar24 offer upgraded accounts for anyone who feeds data. On the Flightradar24 side, they give you a free Business account which is the highest level they have. It’s totally overkill for a hobbiest, but being able to view two years of history or make your own custom fleets is a nice bonus. As long as you keep feeding data, you can enjoy the upgraded account.

### The Impact of the Global Pandemic
Covid-19 is having a severe impact on the number of flights in the sky over our area. When I first activated my receiver I would see hundreds of flights an hour. Over the course of March and April, that dwindled down to just a handful with private planes and cargo flights making up a lot of the traffic I was tracking.

Over the last few weeks, the number of flights I’m tracking has been slowly rising. Some days I see as many as 500 aircraft now and at peak times the number of flights tracked in an hour is more than 50. That’s still about 20% of what it was pre-Covid, but it is interesting to watch as air traffic slowly returns.
