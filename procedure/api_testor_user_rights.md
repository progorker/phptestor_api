```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
 [procedure] api_testor_user_rights
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_user_rights( $p_token, &$p_api_call, &$p_user_make, &$p_user_demo, &$p_storage_full ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: b85a5d3319a9c02433cf442ef184c79a

    ----------------------------

$) $api_call = false; $user_make = false; $user_demo = false; $storage_full = false; \phptestor\api_testor_user_rights( $token, $api_call, $user_make, $user_demo, $storage_full ); echo "\n", "Api Call: ", ($api_call ? 'yes' : 'no'), "\n", "User Make: ", ($user_make ? 'yes' : 'no'), "\n", "User Demo: ", ($user_demo ? 'yes' : 'no'), "\n", "Storage Full: ", ($storage_full ? 'yes' : 'no'), "\n";

    ----------------------------

Api Call: yes
User Make: no
User Demo: yes
Storage Full: no

    ----------------------------
```