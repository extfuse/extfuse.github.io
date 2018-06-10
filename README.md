### Description

User file systems offer numerous advantages over their in-kernel
implementations, such as ease of development and better system reliability.
However, the heavy performance penalty incurred during their user is also well
known.  We observe that existing user file system frameworks are highly general:
they implement a minimal interposition layer in the kernel that simply forwards
all low-level requests to the user-space.  While the design enables a number of
usecases, it severely degrades performance due to frequent kernel-user context
switching.

This work introduces ExtFUSE, a framework for developing extensible user file
systems that also allows applications to register "thin" specialized request
handlers in the kernel to meet their specific operative needs, while retaining
the complex functionality in user-space. 

### Homepage

[Homepage is hosted here](https://extfuse.github.io)
