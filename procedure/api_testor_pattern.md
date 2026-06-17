```
===========_____=======_============
  _ __ _  |_   _|__ __| |_ ___ _ _ 
 | '  \ || || |/ -_|_-<  _/ _ \ '_|
 |_|_|_\_, ||_|\___/__/\__\___/_|  
=======|__/=========================
   API References of phpTestor
           ----- oOo -----
   [procedure] api_testor_pattern
====================================


-------|__/-------------------------
               SYNTAX
------------------------------------

function \phptestor\api_testor_pattern( $p_module, $p_kind, $p_code, $p_variant, &$p_pattern ) {
}


-------|__/-------------------------
               USAGE
------------------------------------

$) $module = 'mytestor'; $kind = 'procedure'; $code = 'api_testor_login'; $variant = 'scrp'; $pattern = ''; \phptestor\api_testor_pattern( $module, $kind, $code, $variant, $pattern ); echo "\n", "Pattern: ", "\n", $pattern, "\n";

    ----------------------------

Pattern: 
set @v_token = '_';
set @v_username = 'mytestor';
set @v_password = 'rzutomqahegpnyx';
call api_testor_login( @v_token, @v_username, @v_password ); select @v_token as `Token`;
call api_testor_logout( @v_token );

    ----------------------------

```