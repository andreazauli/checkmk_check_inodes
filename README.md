checkmk_check_inode
===================

title: Check the inodes state
-----------------------------
* agents: linux
* author: Andrea Zauli <andrea@biodec.com>
* license: GPL
* distribution:
* description:
   Checks the filesystem usage with respect the poin of view of the inodes.

* examples:
  * Setting the check:
    It is a client side local check. So it doesn't need any server side parser,
    just copy the agent local plugin (check_inodes) into the client directory:
    /usr/lib/check_mk_agent/local/check_inodes
    and apply an inventory on the server.

* inventory:
  Each host, which provides the results in the check_mk agent local section,
  gets one check per each filesystem.