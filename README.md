<!--Inheritance=== Child will access all the properties which are public and protected in parent class.

extends-->
<?php

 class A
{
private function show()
{
echo "This is method of parent class<br>";
}

 }
class B extends A
{
public function display()
{
echo "This is method inside class B<br>";
$this->show();
}
}
$a = new A;
$b = new B;
//$b->show();
$b->display();

?>
