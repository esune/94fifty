Maxwell Turpin
12/13/2016
Link: https://mhturpin.github.io/94fifty/

    This is a web app for connecting and sending data to the 94Fifty Bluetooth
basketball. It can pair with the basketball without error; however, I have no
way to check if the data is sent properly since the ball doesn't respond. I
believe it doesn't respond because the data I sent wasn't formatted correctly.
I couldn't figure out how the token was generated (the second element in the
data, directly following TYPE).
    I left console.log() debugging output so that anyone wanting to play with
the code will have an easier time understanding what is happening behind the
scenes.

The data_analysis folder contains a sample breakdown of the data from a packet,
the packet capture it came from, and a command line program to help decode a
segment of data. The segment of data must come from a packet captured during a
dribble activity (TYPE = 0x8320). The folder also contains a table that matches
every possible TYPE with its corresponding class.
