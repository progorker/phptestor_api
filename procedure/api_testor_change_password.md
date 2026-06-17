```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
[procedure] api_testor_change_password
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_change_password( $p_token, $p_password ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: 213cc0ad28337b912cdb464e6ec63f22

    ----------------------------

$) $new_password = 'homosapien'; \phptestor\api_testor_change_password( $token, $new_password );

```