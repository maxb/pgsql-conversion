Overall conversion process
==========================

1. Fetch CVS repository:
   $ rsync -azH --delete anoncvs.postgresql.org::pgsql-cvs cvsroot/

2. Run the deaden-generated-files script.

3. Run cvs2git trunk r5270:
   ./cvs2git --options cvs2git.options

   (cvs2git-example.options is an unmodified copy of the upstream example
   config file at the version cvs2git.options is based on, for comparison.)
