```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
  [function] api_testor_has_right
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_has_right( $p_token, $p_right_code ) : bool {
}


    ----------------------------
           $p_right_code
    ----------------------------

+ 'api_call'
+ 'user_make'
+ 'user_demo'
+ 'storage_full'


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: 2eea69d88687f005080265f78afd4e3e

    ----------------------------

$) $right_code = 'api_call'; $right = \phptestor\api_testor_has_right( $token, $right_code ); echo "\n", "Right ($right_code): ", ($right ? 'yes' : 'no'), "\n";

    ----------------------------

Right (api_call): yes

    ----------------------------
```