Pointing port 80 to another port
--------------------------------

Step 1: View current firewall rules.

sudo ipfw show
Step 2: Add port forwarding rule (80 to 8080)

sudo ipfw add 100 fwd 127.0.0.1,8080 tcp from any to any 80 in
If you want to remove your firewall rules run:

sudo ipfw flush
