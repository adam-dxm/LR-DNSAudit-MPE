# LR-DNSAudit-MPE
LogRhythm MPE Rules for the Microsoft-Windows-DNSServer/Audit EventLog
  
These are a collection of MPE rules to parse data from the Microsoft-Windows-DNSServer/Audit Evenlog, on Windows DNS servers (running Server 2019, 2016, or 2012 R2 with update KB2956577 installed (see: https://support.microsoft.com/kb/2956577).  
  
Importing these rules will create a new Windows (XML) log source type called "MS Win Event Log XML - DNSServer Audit", with an abbreviated form of "WinEvtX - DNSAudit" and a log source type ID of 1000000005.  
  
As always, take care when importing custom MPE rules. The MPE Rule, Regex, and Log Source Type IDs in these files will overwrite anything you already have with a conflicting ID. The MPE rules use IDs from 1000000117 to 1000000216 (with gaps), and MPE Rule regex IDs of 1000000019 to 1000000057. If you have conflicting rule/regex IDs, you will need to fix up the files before you import them.
