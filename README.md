# COMS
This code sends 6 arrays of floats over UDP. 

Each of this arrays has a identifier "DATA", a scaler to send the data using only 2 bytes and a checksum. 

On the otherside, the UDP server must receive all the message and then look for the data identifiers, 
cast the respective data into a float, then divide over the scaler to cancel it. 
