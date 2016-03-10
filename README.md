# Unit 1 Assessment

## Assumptions

  * Basic Java
  * Generics in Java
  * Interface in Java
  * List Class
  * ArrayList
  * LinkedList
  * Tests


???

# Unit 1 Assumptions Assessment

?: Which creates a basic array in Java?

( ) `int [] myList = {"1", "2", "3"};`
( ) `int [] myList = (5, 8, 2);`
( ) `int myList [] [] = {4,9,7,0};`
(X) `int myList [] = {4, 3, 7};`

?: Which is a valid declaration of a method in an interface?

(X) `public double methoda();`
( ) `double public methoda();`

?: Please read the following code. What is the output?

```
public void foo( boolean a, boolean b)
{ 
    if( a ) 
    {
        System.out.println("A"); /* Line 5 */
    } 
    else if(a && b) /* Line 7 */
    { 
        System.out.println( "A && B"); 
    } 
    else /* Line 11 */
    { 
        if ( !b ) 
        {
            System.out.println( "notB") ;
        } 
        else 
        {
            System.out.println( "ELSE" ) ; 
        } 
    } 
}
```

( ) If `a` is true and `b` is true then the output is "A && B"
( ) If `a` is true and `b` is false then the output is "notB"
(X) If `a` is false and `b` is true then the output is "ELSE"
( ) If `a` is false and `b` is false then the output is "ELSE"

?: Can a Java Interface ever contain method definitions?

(X) No
( ) Yes
( ) Sometimes

?: When a class implements an interface, what must it do? 

( ) It must redefine each constant from the interface
(X) It must declare and provide a method definition for each method in the interface.
( ) It must declare a variable for each constant in the interface.
( ) It must include a private method for each method in the interface.

?: Is the following a correct way to start out a class definition:

```
public class MyClass implements MyInterface
```

(X) Yes
( ) No

?: What is the output of this program?

```java
 import java.util.*;
    public class genericstack <E> {
        Stack <E> stk = new Stack <E>();
	public void push(E obj) {
            stk.push(obj);
	}
	public E pop() {
            E obj = stk.pop();
	    return obj;
	}
    }
    class Output {
        public static void main(String args[]) {
            genericstack <String> gs = new genericstack<String>();
            gs.push("Hello");
            System.out.print(gs.pop() + " ");
            genericstack <Integer> gs = new genericstack<Integer>();
            gs.push(36);
            System.out.println(gs.pop());
        }
    }
```

( ) Error
( ) Hello
( ) 36
(X) Hello 36

?: Declare and construct an ArrayList with an initial capacity of 20 references to Object.

( ) `Object list(20) = new ArrayList() ;`
( ) `ArrayList list[20] = new ArrayList() ;`
( ) `ArrayList[Object] list = new ArrayList(20) ;`
(X) `ArrayList<Object> list = new ArrayList<Object>(20) ;`

?: Take a look at the following code. What is the capacity of `list` and what is it's size?

```
ArrayList<String> list = new ArrayList<String>(10) ;
list.add( "Ann" );
list.add( "Bob" );
list.add( "Eve" );
```

( ) Capacity: 3, Size: 3
( ) Capacity: 3, Size: 10
(X) Capacity: 10, Size: 3
( ) Capacity: 10, Size: 10

?: Which is faster?

Option 1:

```
ArrayList<String> list = new ArrayList<String>(10) ;
list.add( "Ann" );
list.add( "Bob" );
list.add( "Eve" );
list.get(1);
```

Option 2:

```
LinkedList<String> list = new LinkedList<String>(10) ;
list.add( "Ann" );
list.add( "Bob" );
list.add( "Eve" );
list.get(1);
```

(X) Option 1
( ) Option 2

???

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/quiz' title='Curriculum Overview'>Curriculum Overview</a> on Learn.co and start learning to code for free.</p>

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/quiz'>Quiz</a> on Learn.co and start learning to code for free.</p>
