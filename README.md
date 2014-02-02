testdriver
==========

linuxcnc testdriver for testing get_rtapi_config.
compiling with comp

comment/uncomment the line
	#define  WO_get_rtapi_config
in anotherconstant.comp for switching the issue off/on.


compiling:
	comp --install anotherconstant.comp

testing:
	halrun -V -I -f anotherconstant.hal
	
view logs:
	tailf /var/log/syslog
	
	
