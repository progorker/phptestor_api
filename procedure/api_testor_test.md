```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
   [procedure] api_testor_test
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_test( $p_token, &$p_id, $p_suite_id, $p_case_id, $p_code, $p_condition, $p_message ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: f6e5703e22a6bc53738f9439bb2a40c0

    ----------------------------

$) $suite_id = -1; $suite_code = 'phpTestorTrial'; \phptestor\api_testor_suite( $token, $suite_id, $suite_code ); echo "\n", "Suite ID: ", $suite_id, "\n";

    ----------------------------

Suite ID: 1

    ----------------------------

$) \phptestor\api_testor_clean( $token, $suite_id );

$) $case_id = -1; $case_code = 'test_numbers'; \phptestor\api_testor_case( $token, $case_id, $suite_id, $case_code ); echo "\n", "Case ID: ", $case_id, "\n";

    ----------------------------

Case ID: 1

    ----------------------------

$) $test_id = -1; $test_code = 'greater.1'; $condition = 2 > 1; $message = '[greater.1] test is success!'; \phptestor\api_testor_test( $token, $test_id, $suite_id, $case_id, $test_code, $condition, $message ); echo "\n", "Test ID: ", $test_id, "\n";

    ----------------------------

Test ID: 1

    ----------------------------
```