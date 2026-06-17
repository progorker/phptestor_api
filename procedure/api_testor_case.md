```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
   [procedure] api_testor_case
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_case( $p_token, &$p_id, $p_suite_id, $p_code ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: 34fabd62add2d93895d9b3eb1a55bab5

    ----------------------------

$) $suite_id = -1; $suite_code = 'phpTestorTrial'; \phptestor\api_testor_suite( $token, $suite_id, $suite_code ); echo "\n", "Suite ID: ", $suite_id, "\n";

    ----------------------------

Suite ID: 1

    ----------------------------

$) $case_id = -1; $case_code = 'test_numbers'; \phptestor\api_testor_case( $token, $case_id, $suite_id, $case_code ); echo "\n", "Case ID: ", $case_id, "\n";

    ----------------------------

Case ID: 1

    ----------------------------
```