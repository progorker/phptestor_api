```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
   [procedure] api_testor_error
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_error( $p_token, &$p_id, $p_suite_id, $p_case_id, $p_code, $p_message ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: 5d05e5f2239c8d1147d929aa4f8bcb97

    ----------------------------

$) $suite_id = -1; $suite_code = 'phpTestorTrial'; \phptestor\api_testor_suite( $token, $suite_id, $suite_code ); echo "\n", "Suite ID: ", $suite_id, "\n";

    ----------------------------

Suite ID: 1

    ----------------------------

$) \phptestor\api_testor_clean( $token, $suite_id );

$) $case_id = -1; $case_code = 'test_numbers'; \phptestor\api_testor_case( $token, $case_id, $suite_id, $case_code ); echo "\n", "Case ID: ", $case_id, "\n";

    ----------------------------

Suite ID: 1
Case ID: 1

    ----------------------------

$) $test_id = -1; $test_code = 'exception.1'; $message = '[exception.1] Field is missing!'; \phptestor\api_testor_error( $token, $test_id, $suite_id, $case_id, $test_code, $message ); echo "\n", "Test ID: ", $test_id, "\n";

    ----------------------------

Test ID: 1

    ----------------------------

$) $results = ''; $beauty = false; \phptestor\api_testor_finish( $token, $suite_id, $results, $beauty ); echo "\n", "===== Results: Finished =====", "\n", $results, "\n";

    ----------------------------

===== Results: Finished =====


+--------------+-------------+------------------------------------------------------------------------------------+
| case         | test        | message                                                                            |
+--------------+-------------+------------------------------------------------------------------------------------+
| test_numbers | exception.1 | [exception.1] test (error) is failed. \nMessage: [exception.1] Field is missing!\n |
+--------------+-------------+------------------------------------------------------------------------------------+


+---------+--------+----------------+----+---------------+--------------+------------+------------+
| version | status | code           | id | success_count | failed_count | test_count | case_count |
+---------+--------+----------------+----+---------------+--------------+------------+------------+
| 1       | RED    | phpTestorTrial | 1  | 0             | 1            | 1          | 1          |
+---------+--------+----------------+----+---------------+--------------+------------+------------+


+------------------------------------------+-----------------------------------------------+
| To re-print:                             | To get source file of [a] test case:          |
+------------------------------------------+-----------------------------------------------+
| $) call api_testor_result('_token_', 1); | $) call api_testor_source('_token_', 1, 'a'); |
+------------------------------------------+-----------------------------------------------+

    ----------------------------

```