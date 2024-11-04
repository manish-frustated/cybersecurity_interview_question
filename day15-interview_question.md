**Explain how you would perform an external penetration test from start to finish**

I would first start by reviewing the rules of engagement to confirm scope. Once I know my target IPs, I will perform enumeration on those IPs to validate client ownership of scope. Once that is performed, I will kick off vulnerability scans against those IPs. While my scans are running, I will perform OSINT against the organization, attempting to find known email addresses/format & who works at the organization, which will allow me to compile possible email addresses & usernames for future attacks

I will also perform breached database searches using a tool like DeHashed in order to find known passwords associated with employees of the company. Once that portion of OSINT is complete, I will then identify any login panels that could allow me to spray usernames/passwords as well as perform credential stuffing attacks. I may use a tool like CredMaster to accomplish this. I will confirm the lockout policy with the client prior to performing any attacks

While attacks are running, I will review open ports & vuln scan findings. I will also dig into other OSINT avenues (code repos, S3 buckets, job postings, social media, etc.) as a means of finding other information that may later lead to an attack

Should I successfully compromise an account, I will see what level of access that account has & perform enumeration. If MFA is in place, I will see if it can be bypassed. I may use a tool like GraphRunner to pillage data & perform enumeration

Should I not get in, or be blocked by MFA, I will ask the client to create an account for me as pentests are time limited & I want to make sure I can test everything possible within our time limits. Once an account is provided, I will perform similar tests mentioned before

During testing, I will document findings as I go & update the client daily. Once my testing is complete, I will compile a report to deliver to the client
