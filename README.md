Q.1“Given a string, check if the string is palindrome or not.” A string is
said to be palindrome if the reverse of the string is the same as the string.
public class Pallindromestrng {
    public static void main(String[] args) {
        String s = "ABCDCBA";
        String rev = "";
        for (int i = s.length() - 1; i >= 0; i--) {
            rev = rev + s.charAt(i);

            if (s.equals(rev)) {
                System.out.println("Pallindrome");
            }
        }
        System.out.println(" Not Pallindrome");

    }
}
