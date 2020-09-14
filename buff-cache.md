To free pagecache, use ``echo 1 > /proc/sys/vm/drop_caches``;

To free dentries and inodes, use ``echo 2 > /proc/sys/vm/drop_caches``;

To free pagecache, dentries and inodes, use ``echo 3 >/proc/sys/vm/drop_caches``. Because this is a non-destructive operation and dirty objects
