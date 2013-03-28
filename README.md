cbench1.3
=========

cbench1.3 for benchmarking openflow1.3 enabled controllers.
Supports throughput/latency evaluation of openflow1.3 controllers.
Sends in packet in and expects either of FLOW MOD/PACKET OUT.
No backward compatibility with openflow1.0 controllers,works only with openflow1.3 controllers.

USAGE: Go to openflow/oflops/cbench 

Run ./cbench for cbench related help.U may see help options as below

./cbench --help
help message
USAGE: cbench [option]  # by Siva Badana 2013
   -c/--controller              <str> hostname of controller to connect to     ("localhost")
   -d/--debug                         enable debugging                         (off)
   -h/--help                          print this message                      
   -l/--loops                   <int> loops per test                           (16)
   -M/--mac-addresses           <int> unique source MAC addresses per switch   (100000)
   -m/--ms-per-test             <int> test length in ms                        (1000)
   -p/--port                    <int> controller port                          (6633)
   -r/--ranged-test                   test range of 1..$n switches             (off)
   -s/--switches                <int> fake $n switches                         (16)
   -t/--throughput                    test throughput instead of latency      
   -w/--warmup                  <int> loops to be disregarded on test start (warmup) (1)
   -C/--cooldown                <int> loops to be disregarded at test end (cooldown) (0)
   -D/--delay                   <int> delay starting testing after features_reply is received (in ms) (0)
   -i/--connect-delay           <int> delay between groups of switches connecting to the controller (in ms) (0)
   -I/--connect-group-size      <int> number of switches in a connection delay group (1)
   -L/--learn-dst-macs                send gratuitious ARP replies to learn destination macs before testing (on)
   -o/--dpid-offset             <int> switch DPID offset                       (1)

