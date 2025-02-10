# AppArmor 

AppArmor provides access control to programs running on a Linux system. The tool implements an additional security layer between the applications invoked in the user space and the underlying system functionality.

For example, we can restrict network calls or filesystem interaction. Many Linux distributions (e.g., Debian, Ubuntu, openSUSE) already ship with AppArmor.

Therefore, AppArmor doesn’t have to be installed manually. Linux distributions that do not support AppArmor use Security-Enhanced Linux (SELinux) instead, which takes a similar approach to AppArmor.