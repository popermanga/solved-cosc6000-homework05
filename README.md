Download Link: https://assignmentchef.com/product/solved-cosc6000-homework05
<br>
Develop a class called <strong>USLength</strong> that is an abstract data type (ADT) for a length. The complete class will include all the following <strong>public member functions</strong> :

A constructor to set yards, feet and inches; ex. 2yd 2ft 3in can be set as <strong>USLength item1(2,2,3)</strong>;

A constructor to set feet and inches; ex.  4ft 3in can be set as <strong>USLength item1(4,3)</strong>;

A constructor to set inches; ex.  23in can be set as <strong>USLength item1(23)</strong>;

A default constructor (takes no input) that sets 0yd 0ft 0in.

Public member function, “<strong>getYards()</strong>” that returns the yard part of length.

Public member function, “<strong>getFeet()</strong>” that returns the foot part of length. Public member function, “<strong>getInches()</strong>” that returns the inch part of length. Public member function, <strong>setLength(1,2,3)</strong> that sets 1yd 2ft 3in.

You may define private member functions. (helper functions)

It is <strong>your decision</strong> how to store the length information, yard, feet, and inches.

You can assume that yard, feet, and inches are all integers. All member variables must be <strong>private</strong>. Note: 12inches = 1foot, 3feet = 1yard.

Use following main function to test your class.

int main(int argc, const char * argv[]) {

USLength bar1(100);     USLength bar2(3,8);

USLength bar3(3,13);

USLength bar4(1,2,23);




std::cout &lt;&lt; “bar1 : ” &lt;&lt; bar1.getYards() &lt;&lt; ” yards, ” &lt;&lt; bar1.getFeet() &lt;&lt; ” feet, ” &lt;&lt; bar1.getI nches() &lt;&lt; ” inches
”;

std::cout &lt;&lt; “bar2 : ” &lt;&lt; bar2.getYards() &lt;&lt; ” yards, ” &lt;&lt; bar2.getFeet() &lt;&lt; ” feet, ” &lt;&lt; bar2.getI nches() &lt;&lt; ” inches
”;

std::cout &lt;&lt; “bar3 : ” &lt;&lt; bar3.getYards() &lt;&lt; ” yards, ” &lt;&lt; bar3.getFeet() &lt;&lt; ” feet, ” &lt;&lt; bar3.getI nches() &lt;&lt; ” inches
”;

std::cout &lt;&lt; “bar4 : ” &lt;&lt; bar4.getYards() &lt;&lt; ” yards, ” &lt;&lt; bar4.getFeet() &lt;&lt; ” feet, ” &lt;&lt; bar4.getI nches() &lt;&lt; ” inches
”;




USLength bar12;

bar12.setLength(bar1.getYards() + bar2.getYards(), bar1.getFeet() + bar2.getFeet(), bar1.getInches(

)+ bar2.getInches());     std::cout &lt;&lt; “bar12 : ” &lt;&lt; bar12.getYards() &lt;&lt; ” yards, ” &lt;&lt; bar12.getFeet() &lt;&lt; ” feet, ” &lt;&lt; bar12. getInches() &lt;&lt; ” inches
”;     return 0; }

https://tulane.instructure.com/courses/2165899/assignments/13464159           1/2 4/23/2018           Homework 05

The output must be:

You see, for example, ‘bar1’ is set 100 inches and the output shows 2 yards, 2 feet and 4 inches. That is 100/12=8 feet, the remeinder is 4 inches, 8/3=2 yards, the remeinder is 2 feet.