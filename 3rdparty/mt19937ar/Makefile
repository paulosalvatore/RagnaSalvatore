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

# 3rdparty/mt19937ar/Makefile.  Generated from Makefile.in by configure.

MT19937AR_OBJ = mt19937ar.o
MT19937AR_H = mt19937ar.h



CC = gcc
export CC

#####################################################################
.PHONY: all clean buildclean help

all: $(MT19937AR_OBJ)

buildclean:
	@echo "	CLEAN	mt19937ar (build temp files)"
	@rm -rf *.o

clean: buildclean
	@echo "	CLEAN	mt19937ar"

help:
	@echo "possible targets are 'all' 'clean' 'buildclean' 'help'"
	@echo "'all'                 - builds $(MT19937AR_OBJ)"
	@echo "'clean', 'buildclean' - deletes $(MT19937AR_OBJ)"
	@echo "'help'                - outputs this message"

#####################################################################

Makefile: Makefile.in
	@$(MAKE) -C ../.. 3rdparty/mt19937ar/Makefile

%.o: %.c $(LIBCONFIG_H) Makefile
%.o: %.c $(MT19937AR_H)
	@echo "	CC	$<"
	@$(CC) -g -O2 -pipe -ffast-math -fvisibility=hidden -Wall -Wextra -Wno-sign-compare -march=i686 -Wno-unused-parameter -Wno-clobbered -Wempty-body -Wformat-security -Wno-format-nonliteral -Wno-switch -Wno-missing-field-initializers -fno-strict-aliasing -g -DHAVE_EXECINFO  -DMAXCONN=16384 -I../common -DHAS_TLS -DHAVE_SETRLIMIT -DHAVE_STRNLEN -DDEBUG -I/usr/include -DHAVE_MONOTONIC_CLOCK -c $(OUTPUT_OPTION) $<
