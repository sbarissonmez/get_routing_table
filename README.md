# Cisco Routing Table

This program gets routing tables from Cisco XE, NXOS, and ASA devices. It then parses the data and prints the route details.

You can  call the routing table class directly from your program and run conditional statements if desired. For example code visit `main.py`

**Steps:**

1. Create a connection object
2. Create a routing table object
3. Call the class property to access the routing table. Data structure is list of lists

        >>> connection_obj = device_login(ip, username, password, enable)
        >>> table_obj = xe_routing.RoutingIos(netmiko_connection)
        >>> [print(", ".join(i)) for i in table_obj.route_table]