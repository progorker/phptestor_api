```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
   [procedure] api_testor_source
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_source( $p_token, $p_suite_id, $p_case_code, &$p_results, $p_beauty = false ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: 02d7469f8edb7fc8bb803aa35f07b937

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

$) $data = '/tst/test_numbers.php'; $option_code = 'src:test_numbers'; $option_remove = false; \phptestor\api_testor_option( $token, $suite_id, $data, $option_code, $option_remove ); $data = null; \phptestor\api_testor_option( $token, $suite_id, $data, $option_code, $option_remove ); echo "\n", "Option ($option_code): ", $data, "\n"; 

    ----------------------------

Option (src:test_numbers): /tst/test_numbers.php

    ----------------------------

$) $case_code = 'test_numbers'; $results = ''; $beauty = false; \phptestor\api_testor_source( $token, $suite_id, $case_code, $results, $beauty ); echo "\n", "=====] Result: Source [=====", "\n", $results, "\n";

    ----------------------------

=====] Result: Source [=====


+----------+--------------------------------------------------+
| Key      | Value                                            |
+----------+--------------------------------------------------+
| Case     | test_numbers                                     |
| Relative | /tst/test_numbers.php                            |
| Absolute | /bioogr/works/myTestorTrial/tst/test_numbers.php |
| Root     | /bioogr/works/myTestorTrial                      |
+----------+--------------------------------------------------+

    ----------------------------
```