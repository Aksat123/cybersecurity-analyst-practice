#logs:
2025-09-03 14:22:10 | EventID=4625 | Failed login attempt | Username=jdoe_admin | IP=101.123.171.5
2025-09-03 14:22:15 | EventID=4625 | Failed login attempt | Username=jdoe_admin | IP=101.123.171.5
2025-09-03 14:22:22 | EventID=4625 | Failed login attempt | Username=jdoe_admin | IP=101.123.171.5
2025-09-03 14:22:35 | EventID=4625 | Failed login attempt | Username=jdoe_admin | IP=101.123.171.5
2025-09-03 14:22:40 | EventID=4625 | Failed login attempt | Username=jdoe_admin | IP=101.123.171.5
2025-09-03 14:23:01 | EventID=4625 | Failed login attempt | Username=jdoe_admin | IP=101.123.171.5
2025-09-03 14:30:00 | EventID=4624 | Successful login | Username=jdoe_admin | IP=101.123.171.5
2025-09-03 14:31:12 | EventID=4672 | Privilege escalation attempt | Username=jdoe_admin | Process=cmd.exe
2025-09-03 14:31:20 | EventID=1102 | Security log cleared | Username=jdoe_admin

Analysis Task:
1. What attack pattern do you notice?
     The user attempted to enter the credential's detail multiple times to login into the account, the actor guessed the password correctly and changed the escalation attempts.
2. What is the most concerning log entry here?
     [2025-09-03 14:31:20 | EventID=1102 | Security log cleared | Username=jdoe_admin] is the high priority risk because the actor accessed the files and folder of the organization and changed the settings of security logs.
3. Based on your findings, how would you classify the incident severity?
     High (active compromise, immediate action required)
   
