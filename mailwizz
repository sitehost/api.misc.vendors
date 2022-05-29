<?php

$url='https://DOMAIN.com/api/lists?pageNumber=1&perPage=10';

function do_get($url){
    $ch = curl_init();

    curl_setopt($ch, CURLOPT_URL,$url );
    curl_setopt($ch, CURLOPT_RETURNTRANSFER, 1);

    curl_setopt($ch, CURLOPT_HTTPHEADER, array(
        'X-API-KEY:2222222222APIKEYHERE3333333333333'
    ));

    
    $result = curl_exec($ch);
    if (curl_errno($ch)) {
        echo 'Error:' . curl_error($ch);
    }
    curl_close($ch);
    return $result;
}


$url='https://DOMAIN.com/api/index.php/lists/THE_LIST_ID_HERE/subscribers'
$post = array(
    'EMAIL' => 'EMAIL@DOMAIN.com',
    'FNAME' => 'JOHN',
    'LNAME' => 'DOE',
    "OTHER_FIELD_HERE"=>"FIELD_VALUE"
);


function do_post($url,$post = array()){
    $ch = curl_init();

curl_setopt($ch, CURLOPT_URL,$url );
curl_setopt($ch, CURLOPT_RETURNTRANSFER, 1);
curl_setopt($ch, CURLOPT_POST, 1);
curl_setopt($ch, CURLOPT_HTTPHEADER, array(
    'X-API-KEY:2222222222APIKEYHERE3333333333333'
));

curl_setopt($ch, CURLOPT_POSTFIELDS, $post);

$result = curl_exec($ch);
if (curl_errno($ch)) {
    echo 'Error:' . curl_error($ch);
}
curl_close($ch);
return $result;

}
