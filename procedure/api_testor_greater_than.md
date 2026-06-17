```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
[procedure] api_testor_greater_than
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_greater_than( $p_token, &$p_id, $p_suite_id, $p_case_id, $p_code, $p_operand, $p_value ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: 439130cfbb227dfe3a9de2c0c0ea80f8

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

$) $test_id = -1; $test_code = 'greater_than.1'; $dbl_a = 3.5; $dbl_b = 2.5; \phptestor\api_testor_greater_than( $token, $test_id, $suite_id, $case_id, $test_code, $dbl_a, $dbl_b ); echo "\n", "Test ID: ", $test_id, "\n";

    ----------------------------

Test ID: 1

    ----------------------------

$) $results = ''; $beauty = false; \phptestor\api_testor_finish( $token, $suite_id, $results, $beauty ); echo "\n", "===== Results: Finished =====", "\n", $results, "\n";

    ----------------------------

===== Results: Finished =====


+---------+--------+----------------+----+---------------+--------------+------------+------------+
| version | status | code           | id | success_count | failed_count | test_count | case_count |
+---------+--------+----------------+----+---------------+--------------+------------+------------+
| 1       | GREEN  | phpTestorTrial | 1  | 1             | 0            | 1          | 1          |
+---------+--------+----------------+----+---------------+--------------+------------+------------+


+------------------------------------------+-----------------------------------------------+
| To re-print:                             | To get source file of [a] test case:          |
+------------------------------------------+-----------------------------------------------+
| $) call api_testor_result('_token_', 1); | $) call api_testor_source('_token_', 1, 'a'); |
+------------------------------------------+-----------------------------------------------+

    ----------------------------

$) $page_no = 1; $results = ''; $beauty = false; \phptestor\api_testor_success( $token, $suite_id, $page_no, $results, $beauty ); echo "\n", "===== Results: Success =====", "\n", $results, "\n";

    ----------------------------

===== Results: Success =====


+--------------+----------------+-------------------------------------------------------------------------------+
| case         | test           | message                                                                       |
+--------------+----------------+-------------------------------------------------------------------------------+
| test_numbers | greater_than.1 | [greater_than.1] test (greater_than) is success. \nOperand: 3.5\nValue: 2.5\n |
+--------------+----------------+-------------------------------------------------------------------------------+

    ----------------------------

```