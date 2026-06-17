```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
  [function] api_testor_is_online
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_is_online( $p_token ) : bool {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $token = '_'; $username = 'mytestor'; $password = 'rzutomqahegpnyx'; \phptestor\api_testor_login( $token, $username, $password ); echo "\n", "Token: ", $token, "\n";

    ----------------------------

Token: 2eea69d88687f005080265f78afd4e3e

    ----------------------------

$) $online = \phptestor\api_testor_is_online( $token ); echo "\n", "Online: ", ($online ? 'yes' : 'no'), "\n";

    ----------------------------

Online: yes

    ----------------------------
```