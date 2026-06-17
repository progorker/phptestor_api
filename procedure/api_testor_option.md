```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
   [procedure] api_testor_option
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_option( $p_token, $p_suite_id, &$p_data, $p_code, $p_remove ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: 22228254dd3decfb101eab645475591c

    ----------------------------

$) $suite_id = -1; $suite_code = 'phpTestorTrial'; \phptestor\api_testor_suite( $token, $suite_id, $suite_code ); echo "\n", "Suite ID: ", $suite_id, "\n";

    ----------------------------

Suite ID: 1

    ----------------------------

$) \phptestor\api_testor_clean( $token, $suite_id );

$) $data = '/bioogr/works/myTestorTrial'; $option_code = 'src_dir'; $option_remove = false; \phptestor\api_testor_option( $token, $suite_id, $data, $option_code, $option_remove ); $data = null; \phptestor\api_testor_option( $token, $suite_id, $data, $option_code, $option_remove ); echo "\n", "Option ($option_code): ", $data, "\n"; 

    ----------------------------

Option (src_dir): /bioogr/works/myTestorTrial

    ----------------------------
```