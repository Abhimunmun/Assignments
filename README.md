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

Q.4 Given a string, write a program to remove all the whitespaces from the string.


public class Spacermvstr {
    public static void main(String[] args) {
        String str = "Take you forward";
        str = str.replaceAll("\s", "");

        System.out.println("String after removing whitespaces: " + str);
    }
}


Q.5Write a program to remove all characters from a string except alphabets in a given string


public class Problemstr5 {
   public static void main(String[] args)
   {
    String str="take12% *&u ^$#forward";
    String str2=str.replaceAll("[^a-z A-Z]","");
    str2=str2.replaceAll("\\s","");
     System.out.println(str2);
   }
}

Q.6Reverse a String. Write a program that reverses a given string. Problem: Given a string, calculate the sum of numbers in a string (multiple consecutive digits
are considered one number)


public class Problemstr6 {
    public static void main(String[] args) {
        String str = "123xyz";
        String rev = "";
        
  
        for (int i = str.length() - 1; i >= 0; i--) {
            rev = rev + str.charAt(i);
        }
    
        System.out.println(rev);
        int sum = 0;
        for (int i = 0; i < str.length(); i++) {
            char c = str.charAt(i);
            if (Character.isDigit(c)) {
                int digit = Character.getNumericValue(c);
                sum += digit;
            }
        }
        
        System.out.println("Sum of digits: " + sum);
    }
}



