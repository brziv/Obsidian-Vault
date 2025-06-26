#system

7 layers:
Application: 
Presentation:
Session:
Transport:
Network:
Data Link:
	LLC (Logical Link Control): multiplexing, data flow
	MAC (Media Access Control): receiving packets from above, dividing them into frames and passing them (bit-by-bit) to below
	Switch: uses MAC addresses to forward data frames
Physical:
	Signals: encoding-decoding, modulation-demodulation
	Medium: wires, fiber optics, wireless
	Transmission: simple, half duplex, full duplex
	Topology: ring, mesh, star, bus, tree

