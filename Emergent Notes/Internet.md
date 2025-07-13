#system 

Hardware and software components:
	End system (host): devices connected to the Internet
		Internet is basically connecting end systems to each other
		ISP (Internet Service Provider): allow end systems to access the Internet
	.
	Communication link: coaxial cable, copper wire, optical fiber, radio spectrum
	.
	[[Packet switch]]: router, link-layered switch
		Analogy:
			Packet - truck, data - cargo
			Comlink - highway, packet switch - intersection
			End system - building
	.
	Internet standards: IETF -> protocols: TCP, IP, HTTP and more

Infrastructure that provide services to applications:
	Distributed applications: mail, web, social network, messaging, VoIP, streaming, games, P2P file-sharing, remote login and more
		Idea to app: write programs that run on the end systems
	API: set of rules for programs to exchange data with each other
		Alice send a letter to Bob using the postal service. She needs to write Bob's name, address, zip code; seal the envelope, put a stamp, and finally drop the envelope into a mailbox.

Protocols: defines format and order of messages, actions taken on events (transmission, receipt)
	Human: "Hi" -> "Hi" -> "Time?" -> "2:00"
	Network: any activity involves two or more remote entities communicating
		TCP: request -> reply (server) -> GET -> file (web page)