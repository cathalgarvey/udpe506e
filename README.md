# udpe506e  

### Say what?
- A program that sends one UDP packet containing 508 `e` - the maximum safe UDP payload size - to every 
address on the internet.
- eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee
- Uses port 101 (ASCII ordinal of `e`)
- I recommend you don't run it
- AGPL
- Comes with a 32-bit x86 linux binary, because I forgot to add that to the `.gitignore`
- R.I.P [e30e/e98e](https://linuxwit.ch/blog/2018/12/e98e/)

### How do I build it?
Please don't.  
(Use rustc)

### It seems slow. How long should it take to run?
Sending packets to all of IPv4 should take about 6 hours with a fast computer on a gigabit connection.  
Sending them to all of IPv6 (which begins immediately after IPv4 is completed) will take at least 10
septillion years with the same setup. Make sure to run it on a VPS provided by a company that will be 
around a while, like Amazon or Google.  

### How many e will this program send out in total?
If allowed to run until it stops, it will have transmitted precisely 
172,863,442,395,836,739,439,394,300,577,520,094,806,016 `e`, or roughly 1.7 trillion trillion quadrillion 
of them. one teraterapeta-e, if you will.  
  
The actual number of `e` received by the destinations will of course be far less, because UDP does not 
make any guarantees about delivery. Also, the vast majority of IPv6 addresses are unused. One could
sit here and look through the statistics to find a number of `e` expected to ultimately reach their 
destination, but that sounds like a lot of work, and given the scale of the amount of data sent by this
program if it is allowed to finish, it seems unlikely that current statistics about the internet would
even be relevant anyway.

### Will this actually reach every device connected to the internet?
No. This program will attempt to send one UDP packet to every IPv4 and IPv6 address. The specific devices
this includes will vary depending on your local network, but generally speaking, its messages will only
be delivered to devices that have a global IP address, which doesn't include the majority of personal
devices.  
  
More pragmatically speaking, this program will not result in packets being sent to more than a handful
of devices, because you won't run it for long enough to iterate over the majority of the address space.

### Will you help me make a distributed version of this that I can run on a botnet I control?
No.

### Isn't this basically a DDoS attack? You shouldn't be using GitHub to host evil software!
What? No.  
  
This is the opposite of DDoS attack. An effective DDoS involves many computers all sending data to a 
small number of target computers, overwhelming the target with a large volume of requests. This program
sends a single packet to each address on the internet, meaning that each server will receive about one
packet. Since most servers probably won't expect it, their software will just filter it out, and continue
on as normal. It will be like a single-port port scan, except even less invasive, because most servers
will not have anything listening on UDP port 101 (HOSTNAME uses port 101, but I believe this is TCP only),
and the packet will simply be rejected without a reply.  
  
Meanwhile, your computer - the one running this program - will have one of its processor threads loaded
for septillions of years (or until you interrupt it), during which it will also be transmitting a huge 
amount of data that might very well saturate its network upload bandwidth. I suppose you could think of 
this as a "DoS attack" of sorts, but it's not distributed, and the only victim is yourself.

### Won't someone out there be annoyed if anyone runs this, though?
Perhaps so!  
  
Perhaps someone is running a weird experimental UDP service on their public server at port 101, which just 
happens to have a weird buffer overflow vulnerability that makes it crash when it receives a packet 
containing 508 `e`s.  
  
Perhaps Udp Georg, who lives in a cave and subsists only by eating stray UDP packets, will receive such a
windfall of nutrition from this packet full of `e` that he will break out of his cave and rampage across
the countryside, doing millions of dollars in damage before he finally slips on a banana peel and falls 
into another cave.
  
Perhaps some server belonging to the Russian government has an ultra-sensitive IDS watching its UDP ports 
for that evil American nonsense, and the KGB will be dispatched to take you out as soon as this program 
crosses into Russian address space.  
  
Perhaps Cabbage OS, the latest secret Apple prototype for their upcoming IoT line, uses port 101 for its 
covert spy system that receives instructions from Apple HQ, and by sending this packet, you will 
inadvertently uncover a conspiracy that will topple the American tech economy.  
  
It's a big world out there! I have no idea how a given computer will react to being sent a packet full of 
`e`. However, the conventions of networking say that a typical computer receiving an unsolicited,
nonsensical packet out of nowhere will probably just ignore it. Furthermore, if anything does react badly
to being sent a nonsense packet, it probably won't be my fault.

### This page messes with GitHub's web UI! Will you please reduce the number of e?
No. 

### Okay, be level with me. What is this really about?
This is a piece of art with Dadaist inclinations, made very much in the spirit of the original
[e98e](https://github.com/eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee/eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee).
It's not meant to be understood, or to do anything useful, or to make you like me more, or anything. It
needs no purpose, and simply is.  
  
I promise it won't hurt you.
