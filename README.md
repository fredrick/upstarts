#Upstarts

A set of frequently used [Upstart](http://upstart.ubuntu.com/) jobs.
Upstart is "event-based replacement for the /sbin/init daemon" that
enables event driven service management in addition the traditional procedural model of process spawning.

#Usage

Place job definitions in `/etc/init/` and then use `service [job]
[command]` to start/stop/restart/status the services manually. On boot, services flow into each other, only starting if dependent services
have started or asynchronously triggered by system events. For more on [controlling
jobs](http://upstart.ubuntu.com/cookbook/#tools) or Upstart in general
(a [replacement](http://en.wikipedia.org/wiki/Upstart#Adoption) for
System-V `init`), see the
[cookbook](http://upstart.ubuntu.com/cookbook/).

#Author

[Fredrick Galoso](mailto:fgaloso@stackd.com)
