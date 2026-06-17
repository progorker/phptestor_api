```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
 [procedure] api_testor_suite_case
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_suite_case( $p_token, &$p_suite_id, &$p_case_id, $p_suite_code, $p_case_code ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: 721821005206697284b07b7f381d3eb6

    ----------------------------

$) $suite_id = -1; $suite_code = 'phpTestorTrial'; $case_id = -1; $case_code = 'test_numbers'; \phptestor\api_testor_suite_case( $token, $suite_id, $case_id, $suite_code, $case_code ); echo "\n", "Suite ID: ", $suite_id, "\n", "Case ID: ", $case_id, "\n";

    ----------------------------

Suite ID: 1
Case ID: 1

    ----------------------------

```