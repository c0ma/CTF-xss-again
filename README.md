```
<?php
	$x = $_GET['x'];
	$x = preg_replace('/\-\->/','nop', $x);
	$x = preg_replace('/\<s/','nop', $x);
	$x = preg_replace('/\(/','nop', $x);
	$x = preg_replace('/\)/','nop', $x);
	$x = preg_replace('/]/','nop', $x);
	echo "<!--<script>".$x."</script>";
	$xss=$_GET['xss']
	$xss = preg_replace('/(\-\->).(\<s).(\().(\)).(\])/','nop', $xss)
	echo "<!--<script>".$xss."</script>";
  
  /*
  I published the exercise @ swehack.org and in the thread below you can see solutions :)
  https://swehack.org/viewtopic.php?f=37&t=2424
  */
  
?>
```
