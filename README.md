libldb-1.1.15srpm
=================

SRPM building tools for libldb-1.1.15 for runing Samba 4 on RHEL 6.
=======

Required rebuild with libtdb updates for Samba.

These are built from Fedora rawhide releases, and need to be built and
installed in the following order.

	krb5-1.10.3-srpm
	iniparser-3.1-srpm

	libtalloc-2.0.8-srpm
	libtdb-1.2.12-srpm
	libldb-1.1.16-srpm
	libtevent-0.9.18-srpm

	samba-4.0.7-srpm

The "make" command will do these steps.

	make build	# Build the package on the local OS
	make all	# Use "mock" to build the packages with the local
			# samba4repo-6-x96_64 configuration, which needs.
	make install	# Actually install the RPM's in the designated
			# location for samba4repo-6-x86_64


		Nico Kadel-Garcia <nkadel@gmail.com>
