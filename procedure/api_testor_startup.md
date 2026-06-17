```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
   [procedure] api_testor_startup
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_startup() {
  global $g_testor_dir, $g_suite_code, $g_testor_username, $g_testor_password, $g_token, $g_src_dir, $g_suite_id, $g_last_version, $g_clear_version;
}


-------|__/-------------------------
               USAGE
------------------------------------

$) global $g_token, $g_suite_id, $g_testor_dir, $g_suite_code, $g_testor_username, $g_testor_password, $g_last_version, $g_src_dir, $g_clear_version;
$) $g_testor_dir = '/bioogr/psk-19/phpTestor';
$) $g_suite_code = 'phpTestorCheck';
$) $g_testor_username = 'mytestor';
$) $g_testor_password = 'rzutomqahegpnyx';
$) $g_last_version = 0;
$) $g_src_dir = '/bioogr/psk-19/phpTestorCheck';
$) $g_clear_version = false;
$) $g_token = '_';
$) $g_suite_id = -1;

$) \phptestor\api_testor_startup();

$) $v_case_code = 'test_numbers';
$) $v_case_id = -1;
$) \phptestor\api_testor_case( $g_token, $v_case_id, $g_suite_id, $v_case_code );

$) $v_test_code = 'equals.1';
$) $v_test_id = -1;
$) $v_num_a = 30.3;
$) $v_num_b = 30.3;
$) \phptestor\api_testor_equals( $g_token, $v_test_id, $g_suite_id, $v_case_id, $v_test_code, $v_num_a, $v_num_b );

$) \phptestor\api_testor_shutdown();

    ----------------------------

========== Results: Finished ==========


+---------+--------+----------------+----+---------------+--------------+------------+------------+
| version | status | code           | id | success_count | failed_count | test_count | case_count |
+---------+--------+----------------+----+---------------+--------------+------------+------------+
| 2       | GREEN  | phpTestorCheck | 1  | 1             | 0            | 1          | 1          |
+---------+--------+----------------+----+---------------+--------------+------------+------------+


+------------------------------------------+-----------------------------------------------+
| To re-print:                             | To get source file of [a] test case:          |
+------------------------------------------+-----------------------------------------------+
| $) call api_testor_result('_token_', 1); | $) call api_testor_source('_token_', 1, 'a'); |
+------------------------------------------+-----------------------------------------------+


========== Results: Source List ==========


========== Results: Success ==========


+--------------+----------+---------------------------------------------------------------------+
| case         | test     | message                                                             |
+--------------+----------+---------------------------------------------------------------------+
| test_numbers | equals.1 | [equals.1] test (equals) is success. \nOperand: 30.3\nValue: 30.3\n |
+--------------+----------+---------------------------------------------------------------------+


========== Results: Failed ==========


========== Results: Result ==========


+---------+--------+----------------+----+---------------+--------------+------------+------------+
| version | status | code           | id | success_count | failed_count | test_count | case_count |
+---------+--------+----------------+----+---------------+--------------+------------+------------+
| 2       | GREEN  | phpTestorCheck | 1  | 1             | 0            | 1          | 1          |
+---------+--------+----------------+----+---------------+--------------+------------+------------+


+------------------------------------------+-----------------------------------------------+
| To re-print:                             | To get source file of [a] test case:          |
+------------------------------------------+-----------------------------------------------+
| $) call api_testor_result('_token_', 1); | $) call api_testor_source('_token_', 1, 'a'); |
+------------------------------------------+-----------------------------------------------+

    ----------------------------

```