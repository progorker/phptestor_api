```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
   [procedure] api_testor_true
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_true( $p_token, &$p_id, $p_suite_id, $p_case_id, $p_code, $p_condition ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: d91493871b4c9e9e05a161eb9f71dff5

    ----------------------------

$) $suite_id = -1; $suite_code = 'phpTestorTrial'; \phptestor\api_testor_suite( $token, $suite_id, $suite_code ); echo "\n", "Suite ID: ", $suite_id, "\n";

    ----------------------------

Suite ID: 1

    ----------------------------

$) \phptestor\api_testor_clean( $token, $suite_id );

$) $suite_id = -1; $suite_code = 'phpTestorTrial'; $case_id = -1; $case_code = 'test_numbers'; \phptestor\api_testor_suite_case( $token, $suite_id, $case_id, $suite_code, $case_code ); echo "\n", "Suite ID: ", $suite_id, "\n", "Case ID: ", $case_id, "\n";

    ----------------------------

Suite ID: 1
Case ID: 1

    ----------------------------

$) $test_id = -1; $test_code = 'greater.1'; $condition = 2 > 3; \phptestor\api_testor_true( $token, $test_id, $suite_id, $case_id, $test_code, $condition ); echo "\n", "Test ID: ", $test_id, "\n";

    ----------------------------

Test ID: 2

    ----------------------------

$) $results = ''; $beauty = false; \phptestor\api_testor_finish( $token, $suite_id, $results, $beauty ); echo "\n", "===== Results: Finished =====", "\n", $results, "\n";

    ----------------------------

===== Results: Finished =====


+--------------+-----------+---------------------------------------------------------------------+
| case         | test      | message                                                             |
+--------------+-----------+---------------------------------------------------------------------+
| test_numbers | greater.1 | [greater.1] test (true) is failed. \nCondition: 0\nExpected: true\n |
+--------------+-----------+---------------------------------------------------------------------+


+---------+--------+----------------+----+---------------+--------------+------------+------------+
| version | status | code           | id | success_count | failed_count | test_count | case_count |
+---------+--------+----------------+----+---------------+--------------+------------+------------+
| 2       | RED    | phpTestorTrial | 1  | 0             | 1            | 1          | 1          |
+---------+--------+----------------+----+---------------+--------------+------------+------------+


+------------------------------------------+-----------------------------------------------+
| To re-print:                             | To get source file of [a] test case:          |
+------------------------------------------+-----------------------------------------------+
| $) call api_testor_result('_token_', 1); | $) call api_testor_source('_token_', 1, 'a'); |
+------------------------------------------+-----------------------------------------------+

    ----------------------------

```