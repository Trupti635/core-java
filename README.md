package com.practiceex;
import java.util.Scanner;
public class StringEx {

	public static void main(String[] args) {
		Scanner sc= new Scanner(System.in);
		
		// Take input from user
		System.out.print("Enter a String:"); //(e.g Trupti@1999)
         String input= sc.nextLine();
         
         // Variable to store separate parts
         String letters="";
         String Digits =" ";
         String SpecialChars="";
         
         //Loop through each Character
         for(int i=0; i<input.length();i++) {
        	 char ch=input.charAt(i);
        	 if( Character.isLetter(ch)) {
        		 letters+=ch;
        	 } else if(Character.isDigit(ch)) {
        		 Digits +=ch;
        	 }else {
        		 SpecialChars +=ch;
        		  
        	 }
         }
         System.out.println("Leters(String) :"+letters);
         System.out.println("Digits(String) :"+Digits);
         System.out.println("SpecialChars :"+SpecialChars);
         sc.close();
	}

}
