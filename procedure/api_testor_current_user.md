```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
[procedure] api_testor_current_user
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_current_user( $p_token, &$p_user_id, &$p_username ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: 1c458a26963d854f24528905dd876353

    ----------------------------

$) $user_id = -1; $username = '_'; \phptestor\api_testor_current_user( $token, $user_id, $username ); echo "\n", "User ID: ", $user_id, "\n", "Username: ", $username, "\n";

    ----------------------------

User ID: 2
Username: mytestor

    ----------------------------
```