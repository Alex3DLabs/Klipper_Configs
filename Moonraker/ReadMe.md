#  Backup Moonraker Database


Moving Moonraker Database from pi to pi 

How to backup Moonraker Database

You need to install lmdb utilities

apt-get install lmdb-utils

To backup the Moonraker Database run the following command

```
function test() {
  console.log("This code will have a copy button to the right of it");
}
```

mdb_dump -f $HOME/printer_data/database/moonrakerdb.bak -a  $HOME/printer_data/database

Copy the database to your PC/Mac 

On MacOS run 

scp pi@Your.IP.Address.x:~/printer_data/database/moonrakerdb.bak /Users/user_id/Desktop

Once you get the new Pi loaded you can then SCP the file onto it.

scp /Users/alexforadori/Desktop/moonrakerdb.bak pi@192.168.11.159:~/printer_data/database/

Then, on the new Pi run the Moonraker Database restore command

Restore mdb_load -f $HOME/printer_data/database/moonrakerdb.bak -s -T $HOME/printer_data/database

Reboot your Pi or restart the Moonraker service.
