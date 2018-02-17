##############################################################################
#                                                                            #
#                                                                            #
#      Scripts useful for no particular reason.                              #
#                                                                            #
#              Author:  bill@zglue.com                                       #
#                                                                            #
#                                                                            #
##############################################################################

  This repo is to hold scripts or other programs found useful in general dev
  work on Ubuntu.

  Requests for mods or features should be sent to the Author.



upnrf:  Program an nrf52832_dk dev board flash.
        Uses nrfjprog and requires nuttx.hex,
        a softdevice in arch/arm/src/nrf52/softdevice.


clone:  Shortcuts for running "git clone ...." without needing
        to know the url or what branch is useful.

        E.G. clone nuttx  == git clone -b zdk ssh://<$USER>@101.132.142.37:30149/nuttx.git
             clone apps   == git clone -b zdk ssh://<$USER>@101.132.142.37:30149/nuttx_apps.git
             clone micro-ecc == git clone -b master git@github.com/kmackay/micro-ecc.git


aclone: Simply extracts the branch and repo info from a current dir
        and working tree branch and inserts it into the file cdb_clone.

        E.G. Run from the top level of this repo the entry in cdb_clone
        is: git clone -b master git@github.com:zglue-bill/scripts.git

nrf-debug:  Starts JLinkGDBServer for a Nordic nRF52832 device using SWD.

nuttx-debug: Starts gdb to connect to the JLinkGDBServer
