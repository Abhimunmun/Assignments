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

Q.2 Given a string, write a program to count the number of vowels, consonants, and spaces in that string.


public class Checkvowconsstr {
    public static void main(String[] args) {
        String str = "Take u forward is Awesome";
        int vowel = 0;
        int cons = 0;
        int space = 0;
        
        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);
            ch = Character.toLowerCase(ch);
            
            if (ch == ' ') {
                space++;
            } else if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') {
                vowel++;
            } else if (Character.isLetter(ch)) {
                cons++;
            }
        }
        
        System.out.println("Vowels: " + vowel);
        System.out.println("Consonants: " + cons);
        System.out.println("White spaces: " + space);
    }
}


