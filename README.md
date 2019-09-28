RAFT-COMMUNICATE-CHANL package
==============================

The package implements the [`raft-communicate` interface][rc-api] using `CHANL` communication channels.

[rc-api]: https://github.com/nklein/raft/tree/develop/src/communicate/interface

To create an instance, use the following function:

    (defun make-communicate-chanl () ...)

The peer handles must return a `CHANL` channel when passed to the method:

    (defgeneric chanl (peer-handle))
