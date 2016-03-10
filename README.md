Overview
========

A cross-platform module for reboot / restart and shutdown of current system.
If you need it on Linux, 'sudo chmod u+s /sbin/shutdown' 'sudo chmod u+s /sbin/reboot' or modify sudoers file

Usage
-----

Here's an example on how to use this module:

```python
from rebooter import Rebooter

Rebooter(operation='reboot', delay=False, reason=None, force=False)
```

More info
-----

On Mac delay, reason and force are not used.

+ Windows: Uses shutdown command
+ Mac: Uses AppleScript http://apple.stackexchange.com/questions/103571/using-the-terminal-command-to-shutdown-restart-and-sleep-my-mac
+ Linux: uses shutdown or reboot

TODO
-----
+ sleep / hibernate
+ logout


