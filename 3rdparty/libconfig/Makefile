# This file is part of Hercules.
# http://herc.ws - http://github.com/HerculesWS/Hercules
#
# Copyright (C) 2012-2015  Hercules Dev Team
# Copyright (C)  Athena Dev Teams
#
# Hercules is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <http://www.gnu.org/licenses/>.

# 3rdparty/libconfig/Makefile.  Generated from Makefile.in by configure.

LIBCONFIG_OBJ = libconfig.o grammar.o scanctx.o scanner.o strbuf.o
LIBCONFIG_H = libconfig.h grammar.h parsectx.h scanctx.h scanner.h strbuf.h wincompat.h



CC = gcc
export CC

#####################################################################
.PHONY: all clean buildclean help

all: $(LIBCONFIG_OBJ)

buildclean:
	@echo "	CLEAN	libconfig (build temp files)"
	@rm -rf *.o

clean: buildclean
	@echo "	CLEAN	libconfig"

help:
	@echo "possible targets are 'all' 'clean' 'buildclean' 'help'"
	@echo "'all'                 - builds $(LIBCONFIG_OBJ)"
	@echo "'clean', 'buildclean' - deletes $(LIBCONFIG_OBJ)"
	@echo "'help'                - outputs this message"

#####################################################################

Makefile: Makefile.in
	@$(MAKE) -C ../.. 3rdparty/libconfig/Makefile

%.o: %.c $(LIBCONFIG_H) Makefile
	@echo "	CC	$<"
	@$(CC) -g -O2 -pipe -ffast-math -fvisibility=hidden -Wall -Wextra -Wno-sign-compare -march=i686 -Wno-unused-parameter -Wno-clobbered -Wempty-body -Wformat-security -Wno-format-nonliteral -Wno-switch -Wno-missing-field-initializers -fno-strict-aliasing -g -DHAVE_EXECINFO -DPACKAGE_NAME=\"\" -DPACKAGE_TARNAME=\"\" -DPACKAGE_VERSION=\"\" -DPACKAGE_STRING=\"\" -DPACKAGE_BUGREPORT=\"\" -DPACKAGE_URL=\"\" -DSTDC_HEADERS=1 -DHAVE_SYS_TYPES_H=1 -DHAVE_SYS_STAT_H=1 -DHAVE_STDLIB_H=1 -DHAVE_STRING_H=1 -DHAVE_MEMORY_H=1 -DHAVE_STRINGS_H=1 -DHAVE_INTTYPES_H=1 -DHAVE_STDINT_H=1 -DHAVE_UNISTD_H=1 -D__EXTENSIONS__=1 -D_ALL_SOURCE=1 -D_GNU_SOURCE=1 -D_POSIX_PTHREAD_SEMANTICS=1 -D_TANDEM_SOURCE=1 -DHAVE_USELOCALE=1 -DHAVE_NEWLOCALE=1 -DHAVE_FREELOCALE=1 -DHAVE_XLOCALE_H=1 -DHAVE_EXECINFO_H=1 -DHAVE_LIBPCRE=1  -DMAXCONN=16384 -I../common -DHAS_TLS -DHAVE_SETRLIMIT -DHAVE_STRNLEN -DDEBUG -I/usr/include -DHAVE_MONOTONIC_CLOCK -c $(OUTPUT_OPTION) $<
