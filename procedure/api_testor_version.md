```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
   [procedure] api_testor_version
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_version( $p_token, $p_suite_id, $p_cur_ver ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: 9db12c129a44babcc685a8d5233862b6

    ----------------------------

$) $suite_id = -1; $suite_code = 'phpTestorTrial'; \phptestor\api_testor_suite( $token, $suite_id, $suite_code ); echo "\n", "Suite ID: ", $suite_id, "\n";

    ----------------------------

Suite ID: 5

    ----------------------------

$) \phptestor\api_testor_clean( $token, $suite_id );

$) $option_code = 'ver:cur'; $option_remove = true; $data = null; \phptestor\api_testor_option( $token, $suite_id, $data, $option_code, $option_remove ); $version = 15; \phptestor\api_testor_version( $token, $suite_id, $version ); $option_remove = false; $data = null; \phptestor\api_testor_option( $token, $suite_id, $data, $option_code, $option_remove ); echo "\n", "Option ($option_code): ", $data, "\n"; 

    ----------------------------

Option (ver:cur): 15

    ----------------------------
```