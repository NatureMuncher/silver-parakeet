# silver-parakeet

MySQL Database dump script

```
#- dumpdb.sh 0.92.1
## Usage: dumpdb.sh [-d directory] [-f] [-c] [-e] [-h] [-v] [-debug]
##
##       -d <dir> Set dump directory
##       -f       Force regardless of date
##       -c       Compress while dumping (uses less disk at the cost of more CPU/RAM)
##       -e       Enable Extended Insert for large tables (over ${EXTENDED_INSERT_MIN_SIZE} MB)
##       -h       Show help options.
##       -v       Print version info.
##       -debug   Enable debug.
##
## Example:
##
##      dumpdb.sh -cd dump_destination_folder
##
##

# This dump script will create hostname.database.table.sql.gz files which are compressed with
# pigz rsyncable compression. Innodb tables are dumped using --single-transaction.
# There will be server-side configuration files which will allow setting a 
# specific database or a database.table to be skipped.
# This was ported from:
# http://stackoverflow.com/questions/10867520/mysqldump-with-db-in-a-separate-file/26292371#26292371
# with some changes to fit our requirements
```
