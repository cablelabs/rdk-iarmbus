##########################################################################
# If not stated otherwise in this file or this component's Licenses.txt
# file the following copyright and licenses apply:
#
# Copyright 2016 RDK Management
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
##########################################################################

SUBDIRS =

CC = $(CXX)

INCLUDE_FILES = -I../include \
	      -I$(abs_top_srcdir)/core \
              -I${abs_top_srcdir}/core/include \
              -I${abs_top_srcdir}/template/include \
              -I=/usr/include/rdk/iarmbus

AM_CPPFLAGS = $(INCLUDE_FILES)

bin_PROGRAMS = sampleApp

sampleApp_SOURCES = sampleApp.c
sampleApp_LDADD = -lpthread \
                   $(abs_top_builddir)/core/libIARMBus.la
sampleApp_CFLAGS = $(INCLUDE_FILES)
