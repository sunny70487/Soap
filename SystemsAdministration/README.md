# Windows System Administration

## Security Access Tokens
A user's Security Access Token (SAT) is attached to every process launched by the user. It represents what they are authorized to do and is generated by the Local Security Authority Subsystem Service (LSASS). A SAT includes the following elements:
* User's SID
* SIDs of user's global/local group memberships
* SID of user's integrity level
* Privileges on the local system
* Active Directory attributes

## Integrity Levels
Mandatory Integrity Control (MIC) allows the Windows kernel to “...enforce new access control restrictions that cannot be defined by granting user or group permissions in access control lists (ACLs).” MIC represents Microsoft’s implementation of the Biba Mandatory Access Control (MAC) model and is enforced prior to file permissions. MIC labels, also known as mandatory labels, integrity labels, or integrity levels, prevent processes of lower integrity from reading, writing, and/or executing objects of higher integrity. MIC labels are also partly determined by the type of privileges allocated to a user. A user’s integrity level will be one of the following: 
* System: SYSTEM
* High: administrator
* Medium: standard
* Low: very restricted

## Privileges 

## User Account Control

## File Permissions

## Logon Rights

## References
* https://isc.sans.edu/forums/diary/Limiting+Exploit+Capabilities+by+Using+Windows+Integrity+Levels/10531/