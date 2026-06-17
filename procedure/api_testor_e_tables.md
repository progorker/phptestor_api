```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
  [procedure] api_testor_e_tables
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_e_tables( $p_mysql_database, $p_find, &$p_names ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $mysql_db = 'mytestor'; $mysql_find = ''; $names = ''; \phptestor\api_testor_e_tables( $mysql_db, $mysql_find, $names ); echo "\n", "Tables: ", $names, "\n";

    ----------------------------

Tables: temp_names_table , testor_welcome

    ----------------------------

```