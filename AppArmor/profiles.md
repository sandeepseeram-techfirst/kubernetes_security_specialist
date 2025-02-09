# AppArmor Profiles

The profile mode determines the treatment of rules at runtime should a matching event happen. AppArmor distinguishes two types of profile modes:

Enforce
The system enforces the rules, reports the violation, and writes it to the syslog. You will want to use this mode to prevent a program from making specific calls.

Complain
The system does not enforce the rules but will write violations to the log. This mode is helpful if you want to discover the calls a program makes.