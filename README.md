# location-by-ip
location by ip address usinng php



$ip            = "43.251.95.206";//$_SERVER['SERVER_ADDR'];
$details       = json_decode(file_get_contents("http://ipinfo.io/{$ip}"));
$trace_country = $details->country; // -> "IN"

