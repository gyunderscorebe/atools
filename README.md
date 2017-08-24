# Admin tools for AssaultCube (v0.5.0)

## Installation

Download `atools.cfg` and put it into `config/` directory and add `exec config/atools.cfg` to `autoexec.cfg`.

## Configuration

The script needs to know which admin passwords to use on which servers. To do that, it organizes servers into groups that share same password. Press `X` to open `atools` menu.
Inside `Manage server groups` menu you can add new server groups or edit in passwords for predefined ones (w00p, frag.gq, etc.). Each group has a sub menu where you can add server information. It may be easier to use top-level `Add current server` menu that automatically fills in IP and port from current server.

Alternatively, put `atools_group` and `atools_server` commands after `exec config/atools.cfg` in `autoexec.cfg`, see below.

## Commands

* `aban CN [REASON]` - instant ban by client number.
* `abanname NAME [REASON]` - instant ban by name.
* `abanip IP [REASON]` - instant ban by (partial) IP.
* `akick CN REASON` - instant kick by client number.
* `whoare` - list IPs of all players without claiming admin.
* `awhoare` - list full IPs of all players.
* `findcnbyip` - get client number by (partial) IP.
* `claimadmin` - claim admin.
* `withadmin COMMAND` - execute a command as admin.
* `atools_group NAME [PASSWORD]` - add a server group, or set password if it already exists.
* `atools_server IP PORT [DESCRIPTION]` - add a server to the last added server group, or set description if it already exists.
