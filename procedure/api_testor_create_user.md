```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
 [procedure] api_testor_create_user
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_create_user( $p_token, $p_username, $p_password, $p_api_call, $p_user_make, $p_user_demo, $p_quota ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: 29b8a68725bb4c03dd5f3995a668ff0f

    ----------------------------

$) $new_username = 'demo'; $new_password = 'homosapien'; $api_call = true; $user_make = false; $user_demo = false; $quota = 1024 * 1024 * 768; \phptestor\api_testor_create_user( $token, $new_username, $new_password, $api_call, $user_make, $user_demo, $quota );

```