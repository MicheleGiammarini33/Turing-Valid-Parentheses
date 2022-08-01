import java.util.*;
import java.lang.*;
import java.util.Stack;

class Solution {
/**
* @param str: String to be tested for validity
* @return boolean: Returns true if the string is valid e
*/
public static boolean isValid(String s) {
if (s.isEmpty())
{
return true;
} else{

Stack<Character> stack = new Stack<>();
for (int i=0;i < s.length();i++){
char current = s.charAt(i);
if(current == '(' || current == '[' || current == '{' ){
stack.push(current);
} else
{
if (stack.isEmpty()){
return false;
}
char peekChar = stack.peek();


if (
(current == ')' && peekChar != '(')
||(current == '}' && peekChar != '{')
||(current == ']' && peekChar != '[')
) {return false;
}else {
stack.pop();
}
}
}
return true;
}
}
}
public class Main {
public static void main(String args[]) {
Scanner sc = new Scanner(System.in);
String s = sc.nextLine();
if (Solution.isValid(s)) {
System.out.println("valid");
} else {
System.out.println("invalid");
}
}
}
