# Unit 1 Assessment

Throughout this course we assume that students understand a few basic Java concepts. Just like other programmers, we believe that well documented assumptions are incredibly important. Below is roughly what we expect students to know before going through this unit. We've included links to outside resources that we like to learn those individual concepts. After the list of assumptions is a quick quiz. This quiz *should be easy*. If you get any of them wrong or find this quiz hard, please refer to the resources provided to get a quick refresher on any of the topics.

## Assumptions

  * [Basic Java](http://www.amazon.com/Head-First-Java-2nd-Edition/dp/0596009208)
  * [Generics in Java](http://howtodoinjava.com/core-java/generics/complete-java-generics-tutorial/)
  * [Interface in Java](http://www.tutorialspoint.com/java/java_interfaces.htm)
  * [Collections Framework](http://www.wideskills.com/java-tutorial/java-collections-framework)
  * [ArrayList](http://www.wideskills.com/java-tutorial/java-collections-framework)
  * [LinkedList](https://www.cs.cmu.edu/~adamchik/15-121/lectures/Linked%20Lists/linked%20lists.html) | [LinkedList Resource 2](http://beginnersbook.com/2013/12/difference-between-arraylist-and-linkedlist-in-java/)
  * [JUnit Tests](http://www.vogella.com/tutorials/JUnit/article.html)
  * [Hamcrest Matchers](http://edgibbs.com/junit-4-with-hamcrest/) | [Hamcrest Resource 2](https://springframework.guru/unit-testing-junit-part-3-hamcrest-matchers/)


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

( ) No
(X) Yes
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
            genericstack <Integer> gs2 = new genericstack<Integer>();
            gs2.push(36);
            System.out.println(gs2.pop());
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
// `arrayList` is an instance of ArrayList<String>
// with elements `"Ann"`, `"Bob"`, `"Eve"`
arrayList.get(1);
```

Option 2:

```
// `linkedList` is an instance of LinkedList<String>
// with elements `"Ann"`, `"Bob"`, `"Eve"`
linkedList.get(1);
```

(X) Option 1
( ) Option 2

?: Which of the following method of TestCase class sets up the test, for example, creating test data?

( ) `void setTestName()`
(X) `void setUp()`
( ) `void setUpFixture()`
( ) `void setTestCase()`

?: Given the following code, which Hamcrest matcher will pass?

```
 List<Integer> list = Arrays.asList(5, 2, 4);
```

( ) `assertThat(list, hasSize(3));`
( ) `assertThat(list, contains(5, 4, 2))`
( ) `assertThat(list, containsInAnyOrder(2, 4));`
( ) All of the above
( ) The 1st and 2nd option
(X) The 1st and 3rd option


???

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/java-unit1-assessment'>Java Unit1 Assessment</a> on Learn.co and start learning to code for free.</p>
