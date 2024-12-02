# 24645_Ass2_PluggabeDB
#Below are Queries for creating pluggable databases
CREATING PLUGGABLE DATABASE
-----------------------------------------------------------
CREATE PLUGGABLE DATABASE plsql_class2024db
ADMIN USER el_plsqlauca IDENTIFIED BY Wallen14
FILE_NAME_CONVERT = (
    'D:\SEMISTERS\SEMISTER8\PLSQL\ORADATA\XE\',
    'D:\SEMISTERS\SEMISTER8\PLSQL\ORADATA\XE\PLSQL_CLASS2024DB\'
);


Pluggable database created.

CREATING PLUGGABLE DATABASE TO DELETE
-------------------------------------------------------------------------------
SQL> CREATE PLUGGABLE DATABASE el_to_delete_pdb
  2    ADMIN USER el_plsqlauca IDENTIFIED BY Wallen14
  3    FILE_NAME_CONVERT = (
  4        'D:\SEMISTERS\SEMISTER8\PLSQL\ORADATA\XE\',
  5        'D:\SEMISTERS\SEMISTER8\PLSQL\ORADATA\XE\PLSQL_CLASS2024DB\el_to_delete_pdb\'
  6    );

Pluggable database created.  

#Below are queries used to delete pluggable database
-----------------------------------------------------

SQL> DROP PLUGGABLE DATABASE el_to_delete_pdb INCLUDING DATAFILES;

Pluggable database dropped.
