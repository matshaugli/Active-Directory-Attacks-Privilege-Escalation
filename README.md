# Active Directory Exploitation Lab

## Objective

The objective of this lab was to analyze and exploit vulnerabilities within an Active Directory environment in order to gain elevated privileges. The assessment focused on enumerating domain services, identifying misconfigurations, and leveraging common Active Directory attack techniques to escalate privileges and compromise domain resources.

This exercise provided practical experience in understanding how attackers move laterally within Windows domains and how weaknesses in authentication mechanisms can be exploited.

### Skills Learned

- Enumerating users, groups, and domain privileges within Active Directory environments.
- Identifying common AD misconfigurations that allow privilege escalation.
- Understanding and exploiting Kerberos authentication weaknesses.
- Performing credential attacks such as AS-REP Roasting and Kerberoasting.
- Using graph-based analysis to visualize privilege escalation paths.
- Executing lateral movement techniques within a compromised domain environment.
- Understanding domain compromise techniques such as DCSync attacks.

### Tools Used

- **BloodHound** for analyzing Active Directory attack paths and privilege escalation routes.
- **LDAP enumeration tools** for querying domain objects.
- **SMB tools** for interacting with file shares and authentication services.
- **Kerberos attack techniques** including AS-REP Roasting and Kerberoasting.
- **Credential exploitation techniques** such as Pass-the-Hash.
- **Windows domain environment** for testing Active Directory vulnerabilities.

## Steps

### Step 1 – Initial Enumeration

The first step involved identifying domain users, groups, and available services. Enumeration techniques were used to gather information about the Active Directory environment and discover potential entry points.


### Step 2 – LDAP Enumeration

LDAP queries were used to extract detailed information about users, groups, and permissions within the domain. This information helped identify accounts with misconfigurations or elevated privileges.


### Step 3 – Kerberos Attacks

Kerberos-based attacks were performed to obtain password hashes from domain accounts.

Techniques used included:

- **AS-REP Roasting**
- **Kerberoasting**

These attacks target weaknesses in Kerberos authentication configurations.


### Step 4 – BloodHound Analysis

BloodHound was used to visualize relationships between users, groups, and permissions within the Active Directory environment.

This allowed identification of possible **privilege escalation paths** leading to higher-level domain access.


### Step 5 – Credential Exploitation

Captured credentials and hashes were used to authenticate to additional systems within the domain using techniques such as:

- Pass-the-Hash
- SMB authentication attacks

This allowed further lateral movement inside the network.


### Step 6 – Domain Privilege Escalation

The final stage involved exploiting domain privileges to achieve higher levels of access within the environment. Techniques such as **DCSync attacks** were used to simulate domain compromise.


### Project Link
[Active Directory Exploitation](Ethical_Hacking_A2.pdf)
