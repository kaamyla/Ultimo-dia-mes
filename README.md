<?php

function ultimo_dia_mes($periodo){

	list($dia,$mes,$año)=explode('-',$periodo);

	$mes = mktime( 0, 0, 0, $mes, 1, $año);
	
	$ultimo_dia = intval(date("t",$mes));
	
	return $ultimo_dia;
	
}

?>
