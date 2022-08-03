# Stacks
Stacks
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner sc=new Scanner(System.in);
	    String s=sc.nextLine();
	    Stack<Character> st=new Stack<>();
	    for(int i=0;i<s.length();i++){
	        char ch=s.charAt(i);
	        if(ch==')'){
	            if(st.peek()=='('){
	                System.out.println("true");
	                return;
	            }
	            else{
	                while(st.peek()!='('){
	                    st.pop();
	                }
	            }
	            
	        }
	        else{
	            st.push(ch);
	        }
	    }
	    System.out.println("false");
		
	}
}
