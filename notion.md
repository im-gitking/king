💡
Inputs
Scanner class is used to take inputs in Java.
Fist we need to import util package for using Scanner class by
import java.util.*; → * means we are importing everything of that package
Then we need to create a new object sc of scanner class → 
Scanner sc = new Scanner(System.in);
Like System.out in Output → Here we need to write System.in
Then next() function helps, sc object to catch input given by User →
String name = sc.next();
next() function has many variants ->
next() → Captures until a space.
nextLine() → Captures a whole String with spaces also.
nextInt() → Captures Integers.
nextFloat() → Captures Float.
nextDouble() → Captures Double.
nextBoolean() → Captures Boolean.
nextShort() → Captures Short.
nextLong() → Captures Long.
Example:
1
2
3
4
5
6

7

8
9
10
import java.util.*;

public class JavaNew {
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        String a = sc.next();
        System.out.println(a);
    }
}
​
