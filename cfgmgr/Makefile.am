INCLUDES = -I $(top_srcdir) -I $(top_srcdir)/orchagent
CFLAGS_SAI = -I /usr/include/sai

bin_PROGRAMS = vlanmgrd intfmgrd buffermgrd

if DEBUG
DBGFLAGS = -ggdb -DDEBUG
else
DBGFLAGS = -g
endif

vlanmgrd_SOURCES = vlanmgrd.cpp vlanmgr.cpp $(top_srcdir)/orchagent/orch.cpp $(top_srcdir)/orchagent/request_parser.cpp shellcmd.h
vlanmgrd_CFLAGS = $(DBGFLAGS) $(AM_CFLAGS) $(CFLAGS_COMMON) $(CFLAGS_SAI)
vlanmgrd_CPPFLAGS = $(DBGFLAGS) $(AM_CFLAGS) $(CFLAGS_COMMON) $(CFLAGS_SAI)
vlanmgrd_LDADD = -lswsscommon

intfmgrd_SOURCES = intfmgrd.cpp intfmgr.cpp $(top_srcdir)/orchagent/orch.cpp $(top_srcdir)/orchagent/request_parser.cpp shellcmd.h
intfmgrd_CFLAGS = $(DBGFLAGS) $(AM_CFLAGS) $(CFLAGS_COMMON) $(CFLAGS_SAI)
intfmgrd_CPPFLAGS = $(DBGFLAGS) $(AM_CFLAGS) $(CFLAGS_COMMON) $(CFLAGS_SAI)
intfmgrd_LDADD = -lswsscommon

buffermgrd_SOURCES = buffermgrd.cpp buffermgr.cpp $(top_srcdir)/orchagent/orch.cpp $(top_srcdir)/orchagent/request_parser.cpp shellcmd.h
buffermgrd_CFLAGS = $(DBGFLAGS) $(AM_CFLAGS) $(CFLAGS_COMMON) $(CFLAGS_SAI)
buffermgrd_CPPFLAGS = $(DBGFLAGS) $(AM_CFLAGS) $(CFLAGS_COMMON) $(CFLAGS_SAI)
buffermgrd_LDADD = -lswsscommon

