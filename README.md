# NewYork-Boston-Subnetting-Lab
My first CCNA lab, a basic VLSM configuration lab for two offices(New York and Boston).

Lab Scenario:
- New York location has 2 departments(Engineering and Sales)
- Engineering has 27 hosts plus router interface = 28 hosts
- Sales department has 13 hosts plus router interface = 14

- Boston location 2 departments(Engineering and Sales)
- Engineering has 27 hosts plus router interface = 28
- Sales department has 6 hosts plus router interface = 7 hosts

We've been given the address space 200.15.10.0/24
---- allocate a suitable subnet for each department, starting with the largest segment
---- allocate this subnet at the start of the address space


What I did:
- Subnetted the given address space into smaller networks, suitable for each department (done)
- Configured each router interface with the correct IP address
- Configured Static routes for both routers so they can reach other departments (done)
- Configured IP's for all PC's


Engineering New York and Boston:

Subnet 1: 200.15.10.0 - 200.15.10.31 (New York Engineering Department) /27

Subnet 2: 200.15.10.32 - 200.15.10.63 (Boston Engineering Department) /27


Subnet 3: 200.15.10.64 - 200.15.10.79 (New York Sales Department) /28

Subnet 4: 200.15.10.80 - 200.15.10.95 (Boston Sales Department) /29

Point to Point Link:200.15.10.96 - 200.15.10.99 /30
