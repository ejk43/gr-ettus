# Copyright 2011,2012 Free Software Foundation, Inc.
#
# This file is part of GNU Radio
#
# GNU Radio is free software; you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation; either version 3, or (at your option)
# any later version.
#
# GNU Radio is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with GNU Radio; see the file COPYING.  If not, write to
# the Free Software Foundation, Inc., 51 Franklin Street,
# Boston, MA 02110-1301, USA.

########################################################################
# Install public header files
########################################################################
install(FILES
    api.h
    barrier.h
    device3.h
    rfnoc_block.h
    rfnoc_fir_cci.h
    rfnoc_window_cci.h
    rfnoc_block_impl.h
    rfnoc_radio.h
    rfnoc_generic.h
    rfnoc_fosphor_c.h
    DESTINATION include/ettus
)

if(ENABLE_QT)
    install(FILES
        fosphor_display.h
        DESTINATION include/ettus
    )
endif(ENABLE_QT)
