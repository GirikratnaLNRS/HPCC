################################################################################
#    HPCC SYSTEMS software Copyright (C) 2012 HPCC Systems®.
#
#    Licensed under the Apache License, Version 2.0 (the "License");
#    you may not use this file except in compliance with the License.
#    You may obtain a copy of the License at
#
#       http://www.apache.org/licenses/LICENSE-2.0
#
#    Unless required by applicable law or agreed to in writing, software
#    distributed under the License is distributed on an "AS IS" BASIS,
#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
#    See the License for the specific language governing permissions and
#    limitations under the License.
################################################################################

HPCC_ADD_SUBDIRECTORY (include)
HPCC_ADD_SUBDIRECTORY (jhtree)
HPCC_ADD_SUBDIRECTORY (jlib)

if (NOT JLIB_ONLY)
   HPCC_ADD_SUBDIRECTORY (logaccess)
   HPCC_ADD_SUBDIRECTORY (hrpc)
   HPCC_ADD_SUBDIRECTORY (mp)
   HPCC_ADD_SUBDIRECTORY (security)
   HPCC_ADD_SUBDIRECTORY (xmllib)
   HPCC_ADD_SUBDIRECTORY (xmllibtest "PLATFORM")
   HPCC_ADD_SUBDIRECTORY (masking)
endif( )
