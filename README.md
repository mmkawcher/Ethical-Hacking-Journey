Topic: Recon Report__ Tesla.com 
OS: Kali Linux 
Action: 
1.1 Subdomain Hunting using -sublist3r 
Command used: sublist3r -d tesla.com 
Result: Multiple Subdomains of Tesla.com discoverd. 
1.2 Technology Detection using Whatweb 
Command used: whatweb tesla.com 
Result: IP add,Country,HTTP server Info of Tesla.com 
1.3 Passive Information Gathering using Burp Suite 
I used Burp Suite to intercept & analyze web requests 
Result: Burpsuite provided request & additional passive information about the Website 
1.4 Technology Stack Analysis using Wappalyzer 
I used Wappalyzer to analyze the Technologies used by Tesla.com 
Result: Wappalyzer identified the Framework,payment processing system,security components 
used by Tesla.com 
1.5 Setting up Breach-Parse 
I open the Terminal from /Downloads directory and copied the breach-parse to /opt directory 
Command used: sudo cp -r breach-parse /opt 
Result: breach-parse was successfully copied to the /opt directory  
1.6 Running Breach-parse on Tesla.com 
I switched to root user and ran Breachparse to find leaked credentials related to Tesla.com 
Command used:  
sudo su 
ls 
cd breach-parse 
ss 
chmod +rwx breach-parse.sh 
./breach-parse.sh @tesla.com tesla.txt 
Result: Breachparse successfully ran and found leaked email & Passwords combination related 
to Tesla.com 
#Conclusion: 
In this Task,i performed passive footprinting of Tesla.com using multiple tools .I discovered 
subdomains,identified technology stacks,analyzed web traffic and found leaked credentials 
using Breachparse.These methods are part of passive reconnaissance and help in understanding 
the target without directly attacking it. 
