    Wed. January 9th, 6:53pm at FreeGeek -- 1731 SE 10th Ave.

### Parallel and Distributed Perl

Speaker: Eric Wilhelm

Presenting techniques and tools for parallelizing and distributing
tasks across multiple cores or nodes with perl (and mostly on *nix.)
The focus is on clean architecture, cross-platform clustering, and
removing the distinctions between SMP and clustering.

* basics:          models and laws
* control:         forking/ssh/daemons
* communication:   pipes/NFS/IPC
* management:      waiting, polling, killing
* non-blocking:    iterators, cursors, IO::Select
* bonus:           unionfs+NFS
* if time allows:  threads
