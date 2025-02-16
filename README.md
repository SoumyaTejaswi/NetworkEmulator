# NetworkEmulator
Developed a Network Emulator of a star-wired LAN Topology
#####################################################
# Developped by Soumya Tejaswi Vadlamani and Sai Madhavi Gujju
#
#####################################################

Code is written in python 

commands to run the code
------------------------------------------------------------------------
to run the bridge1 --------> python3 Bridge.py cs1 5 ||
to run the bridge2--------->python3 Bridge.py cs2 5||
to run the bridge3--------->python3 Bridge.py cs3 5 ||
to run the router1--------->python3 Station.py -route ifaces.r1 rtable.r1 hosts ||
to run the router1--------->python3 Station.py -route ifaces.r2 rtable.r2 hosts ||
to run the station A -------->python3 Station.py -no ifaces.a rtable.a hosts ||
to run the station B -------->python3 Station.py -no ifaces.b rtable.b hosts ||
to run the station C -------->python3 Station.py -no ifaces.c rtable.c hosts ||
to run the station D -------->python3 Station.py -no ifaces.d rtable.d hosts ||
------------------------------------------------------------------------

**** please mention the full path of the iface, rtable if they are in other directories

Commands supported in stations/routers/bridges
     stations:

	   send <destination> <message> // send A message
	   show arp 		// show the ARP cache table information
	   show pq 		// show the pending_queue
	   show	host 		// show the IP/name mapping table
	   show	iface 		// show the interface information
	   show	rtable 		// show the contents of routing table
	   quit // close the station

    routers:

	   show	arp 		// show the ARP cache table information
	   show	pq 		// show the pending_queue
	   show	host 		// show the IP/name mapping table
	   show	iface 		// show the interface information
	   show	rtable 		// show the contents of routing table
	   quit // close the router


   bridges:

	   show mac_mapping 		// show the contents of self-learning table
	   quit // close the bridge


*** please run the bridges first then stations or routers
