

Install java agent to monitor the applications based on Java

Get the licesence key

Download the java agent

Unzip the agent file to application home directory (tomcat home directory)

$ java -jar newrelic.jar install

![new\_relic](https://github.com/arunkundrupu1990/new\_relic/blob/master/images/01\_new\_relic.png)

![new\_relic](https://github.com/arunkundrupu1990/new\_relic/blob/master/images/01\_new-relic\_1.png)

Include java agent with jvm argument

To pass the -javaagent argument on Tomcat configure catalina.sh

$ sudo vi catalina.sh

export JAVA\_OPTS=&quot;$JAVA\_OPTS -javaagent:_/opt/tomcat/apache-tomcat-8.5.32/newrelic/_newrelic.jar&quot;

Restarted the application.

On the new relic dashboard select the option &quot;listen for my application&quot;

Then application sends data to new relic.

Got an error :

My application not sending data to new relic.

![new\_relic](https://github.com/arunkundrupu1990/new\_relic/blob/master/images/02\_new\_relic\_error1.png)

Agent is not connecting to collector

![new\_relic](https://github.com/arunkundrupu1990/new\_relic/blob/master/images/03\_new\_relic\_error2.png)

configured the newrelic.yml file and entered the licesence key of new relic

New Relic agent started:

![new\_relic](https://github.com/arunkundrupu1990/new\_relic/blob/master/images/04\_new\_relic\_agent\_started.png)

Response time:

Response time is an average of the total time spent across all web transactions occurring within a selected time frame on the server-side.

Output: 20ms per hour

Throughput:

Throughput is requests per minute through the application.

![new\_relic](https://github.com/arunkundrupu1990/new\_relic/blob/master/images/05\_new\_relic\_output.png)

![new\_relic](https://github.com/arunkundrupu1990/new\_relic/blob/master/images/07\_new\_relic\_response\_time.png)

Deployed jenkins war file on tomcat aplliction server and observed the metrics

![new\_relic](https://github.com/arunkundrupu1990/new\_relic/blob/master/images/06\_new\_relic\_jenkins.png)


