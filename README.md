# SyslogDescription

example:

PRI = 191

To get the Facility
Divide the PRI number by 8. 
191/8 = 23.875
The whole number part is the facility.

To get the Severity
Take the whole number part 23 and multiply by 8 and the product subtract from 191:
191 - (23 * 8 )= 7

PRI = Facility 23 and Priority (7)

Work backword to check our work:
23*8 = 184 + 7 = 191


syslog severity overview

Numerical         Severity
          Code

           0       Emergency: system is unusable
           1       Alert: action must be taken immediately
           2       Critical: critical conditions
           3       Error: error conditions
           4       Warning: warning conditions
           5       Notice: normal but significant condition
           6       Informational: informational messages
           7       Debug: debug-level messages
           
           
Numerical             Facility
          Code

           0             kernel messages
           1             user-level messages
           2             mail system
           3             system daemons
           4             security/authorization messages (note 1)

           5             messages generated internally by syslogd
           6             line printer subsystem
           7             network news subsystem
           8             UUCP subsystem
           9             clock daemon (note 2)
          10             security/authorization messages (note 1)
          11             FTP daemon
          12             NTP subsystem
          13             log audit (note 1)
          14             log alert (note 1)
          15             clock daemon (note 2)
          16             local use 0  (local0)
          17             local use 1  (local1)
          18             local use 2  (local2)
          19             local use 3  (local3)
          20             local use 4  (local4)
          21             local use 5  (local5)
          22             local use 6  (local6)
          23             local use 7  (local7)
