//Security
//Secure Sharing of Information Using an Algorithm Namely KAN
package iss;
import java.util.Scanner;
import java.util.Random;
import java.util.Arrays;


/**
 *
 * @author sadhu narayana naidu
 */
public class ISS {
    public static void main(String []args){
        
        Random r = new Random();
        char[] options = {'$','A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z','@','a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z','#','*','!','%','^','&','(',')','_','-','+','=','~','?','/','[',']','{','}','|','`',':',';',',','.','"'};
        char[] result =  new char[5];
        String decrypted_message="";
        String encrypted_message="";
        String decrypt_message_boggus="";
    String zzz="";
    String yyy="";
    String temp="";
    String zz1="";
    int value=0;
    int value1=0;
    int value2=0;
    int key_encry;
    int[] ar= new int[8000];
    char[] aar= new char[8000];
    int dd=0;
    int q=0;
    String[] final_decrypt=new String[8000];
    String k11="";
    int[] valuear= new int[8000];
    char[] encrypted= new char[8000];
    char[] decrypted= new char[8000];
    String[] arra= new String[8000];
    String[] arra1= new String[8000];
   int[] array_length= new int[8000];
   String[] final_array= new String[8000];
    Random r1=new Random();
    String input;
    String[] ss_decrypted= new String[8000];
        
        int space=3;
        String string="";
        Scanner sc= new Scanner(System.in);
        System.out.println("Enter the string");
        String string1=sc.next();
        System.out.println("Original plain text"+ string1);
        //String string1="SADHUNARAYANANAIDUKAVUTURIT";
        /*if (string.contains(" ")) {
         string=string.replace(" ","@");
         System.out.println("replace sttring"+ string);
        }*/        for(int i=0;i<string1.length();i++)
        {
             string = string1.replaceAll(".......(?!$)", "$0:");
        }
    //System.out.println("========================="+string);
        //String text = "how are you?";
        //String[] textArray= text.splitByNumber(4); 
        //System.out.println(textArray);
        //String inpu="KOPPPSRI";
        //char[] stringArray = inpu.toCharArray();
        //System.out.println("array length"+stringArray.length);
        /*for(int k=0;k<stringArray.length;k++)
        {
            int xy= k*4-1;
            //System.out.println(xy);
            //System.out.println(stringArray[]);
           if(xy<stringArray.length)
            {
                System.out.println(xy);
                if(xy==-1)
                {
                    xy=0;
                }
                //System.out.println(stringArray[xy]);
                String xx=Character.toString(stringArray[xy]);
                xx=xx.replace(xx,stringArray[xy]+"-"); 
                System.out.println(xx);
            }
        }*/
        //System.out.println(stringArray);
        
        //System.out.println(arra1);
    
        String[] parts = string.split(":");
        //System.out.println("split array"+string);
        int xy= parts[1].length();
        String[] arra2= new String[100];
        String zzz1="";
         
         
        //System.out.println("Replaced string "+string);
        //System.out.println("arrya_length"+xy);
        for(int yo=0;yo<parts.length;yo++)
        {
            
           input =parts[yo];
           //System.out.println(input);
        char[] stringToCharArray = input.toCharArray();
        String original= new String(stringToCharArray);
        //System.out.println("stringToCharArray_length"+stringToCharArray.length);
        for(int j=0; j<stringToCharArray.length;j++)
        {
            String k= Character.toString(stringToCharArray[j]);
            for(int i=0;i<space;i++)
            {
            result[i]=options[r1.nextInt(5)];
            String yy= Character.toString(result[i]);
            yyy=yyy+yy;
            }
            zzz=k+yyy;
            yyy="";
            //System.out.println(zzz);
            //for(int q=0;q<stringToCharArray.length;q++)
            // {
            arra[j]= zzz;
            //}
        }
        for(q=0;q<stringToCharArray.length;q++)
        {
            //System.out.println(arra[q]);
        }
        //int sum= (stringToCharArray.length)*space;
        //System.out.println("input length"+input.length());
        int key=(space-1)*(input.length());
        //System.out.println("key"+key);
        String keyalpha= Character.toString(options[key]);
        //System.out.println(keyalpha);
        //System.out.println(stringToCharArray.length);
        String pix1="";
        for(int x=0;x<stringToCharArray.length; x++)
        {
            String lette= arra[x];
            pix1=pix1+lette;
            //System.out.println(pix1);
        }
        zz1= pix1+keyalpha;
        
        //System.out.println("string after concating the key alphabet"+zz1);
         //ENCRYPTION OF EACH LETTER IN THE STRING
        int length_string= zz1.length();
        //System.out.println("length of the string after concating the key value"+length_string);
        int k=length_string;
        //System.out.println("length_string"+length_string);
        int key_len=length_string-1;
		char CharArray[] = zz1.toCharArray();
 	    //System.out.println("printing the string characters using array");
		for (char output : CharArray) 
		{
		    //System.out.println(output);
        }
        //System.out.println(CharArray[k-1]);
        //System.out.println("CharArray.length"+CharArray.length);
        for(int i=0;i<CharArray.length;i++)
        {
            char f=CharArray[i];
            //System.out.println(CharArray[i]);
            //s1.replace('a','e');
            for (int ty = 0; ty < options.length; ty++)
            {
                 if (options[ty] == f)
			    {
			        value= ty;
			    }
            }
            //System.out.println("position of a character in options array"+value);
            
            char tt=options[key_len];
            if(i<length_string-1)
            {
                //System.out.println(value);
		        int i1=value*(length_string-1)/ (key);
		        //System.out.println("value of encrypted message"+i1);
		        char cc1= options[i1];
		       
		         encrypted[i]=cc1;
            }
            else 
            {
                encrypted[i]=f;
            }
		    //System.out.println("encrypted as "+encrypted[i]);
		}
		   //System.out.println("Key Encryption using RSA algorithm");
        int p1=13;
        int q1=5;
        int total=p1*q1;
        int pi= (p1-1)*(q1-1);
        if(total<CharArray.length)
        {
            System.out.println("please choose another prime numbers whose product is greater than the total length of the string");
        }
        else
        {
            //int e = s.nextInt();
            int n1 = pi, e = 3, gcd = 1;

            for(int i = 1; i <= n1 && i <= e; ++i)
            {
                // Checks if i is factor of both integers
                if(n1 % i==0 && e % i==0 && 1<e && e< pi)
                gcd = i;
            }
            if(gcd==1)
            {
                //System.out.printf("G.C.D of %d and %d is %d", n1, e, gcd);
                for(int kt=1;kt<total;kt++)
                {
                    dd=(1+kt*pi/e);
                    System.out.println("dd value"+ dd);
                    if(dd%kt==0)
                    {
                        //System.out.println("To decrypt key d is"+dd);
                        //System.out.println("kt value is "+kt);
            
                        ar[kt]=dd;
                    }
                }
                //System.out.println("dd value"+ar[1]);
            }
            // TO ENCRYPT THE KEY USING RSA
            int chlen=CharArray.length;
          //  System.out.println(chlen);
            char key_ch=encrypted[chlen-1];
           // System.out.println("===================="+encrypted.length);
            for (int tyy = 0; tyy < options.length; tyy++)
            {
                if (options[tyy] == key_ch)
			    {
			        value2= tyy;
			       //System.out.println(value2);
			    }
            }
            //System.out.println("key characters in option array  "+value2);
            //System.out.println("e value "+e);
            //System.out.println("N value "+total);
            int va=value2;
            int ea=e;
            int N=total;
            //System.out.println("Original input  "+ input);
            //System.out.println("plain text after inserted the bogus letters  "+zz1);
            int Cipher= ((value2)^e) % (p1*q1);
			       //System.out.println(Cipher);
           // Cipher=6;
            //System.out.println("Cipher value of last key"+ Cipher);
            char Cipher_text= options[Cipher];
            //System.out.println("Cipher text  "+Cipher_text);
            String b = new String(encrypted);
            int blen= b.length();
            //System.out.println("Cipher text of string"+blen);
		    b = b.replace(b.substring(blen-1), "");
		   
            String str = b;
            //System.out.println(str);
            //System.out.println(str.length());
            str = str.substring(0, chlen-1);
            //System.out.println(str);
            b=str+Cipher_text;
            encrypted_message= encrypted_message+ str; 
          //System.out.println("encrypted_messagge"+encrypted_message);
            //System.out.println("After encryption of key and the letters in the text then the Cipher text is:   "+b);
            
            //System.out.println(dd);
            int Message_value=1+((Cipher^dd)%(total));
            //int Message_value=6;    
            //System.out.println("Message_value "+Message_value);
            char Message_text= options[Message_value];
            //System.out.println(Message_text);
            b = b.substring(0, b.length() - 1) + Message_text;
            //System.out.println("After decryption of key is:   "+b);
            //System.out.println(encrypted);
            for(int i=0;i<chlen;i++)
            {
                char f=encrypted[i];
                //System.out.println(encrypted);
                for (int ty = 0; ty < options.length; ty++)
                {
                    if (options[ty] == f)
			        {
			            value= ty;
			            //System.out.println(value);
			        }
			         
                }
               char tt=options[key_len];
		        int i12=value * Message_value /(length_string-1);
		        //System.out.println(value);
		        //System.out.println(Message_value);
		        //System.out.println(length_string-1);
		        //System.out.println("value of encrypted message"+i12);
		        char cc1= options[i12];
		       
		        decrypted[i]=cc1;
            
		    }
		   // System.out.println(decrypted[0]);
		    String ss= new String(decrypted);
		    //System.out.println("decrypted.length"+decrypted.length);
		    for(int y1=0;y1<chlen;y1++)
		    {
		        ss_decrypted[y1]= ss;
		    }
                    String decryp= new String(ss);
                    decrypt_message_boggus= decrypt_message_boggus+decryp;
         // System.out.println("Before removing boggus letters in between the original string"+ss);
        
        for(int i=0;i<decrypted.length;i++)
        {
            char ch= decrypted[i];
            aar[i] = ch;
            i=i+space;
            //System.out.println(aar[i]);
        }
       //System.out.println("=============================="+aar);
        String sss= new String(aar);
        int blen1= sss.length();
		    sss = sss.replace(sss.substring(blen1-1), "");
            String str1 = sss;
            //System.out.println(str1);
            str1 = str1.substring(0, str1.length()-1);
            if (str1.contains("@")) 
            {
                str1=str1.replace("@"," ");
                
            }
            //System.out.println("Replaced string "+str1);
            final_decrypt[yo]=str1;
          //System.out.println("Finally plain text"+str1);
            //System.out.println("final_decrypt"+final_decrypt[yo]);
            //System.out.println(parts[yo].length());
            array_length[yo]= parts[yo].length();
        }   
    }
        for(int aa=0;aa<parts.length;aa++)
        {
            //System.out.println(array_length[aa]);
        }
        for(int k12=0; k12<parts.length; k12++)
        {
            String s= final_decrypt[k12];
            String upToNCharacters = s.substring(0, Math.min(s.length(), array_length[k12]));
            final_array[k12]=upToNCharacters;
            decrypted_message= decrypted_message+upToNCharacters;
       
       }
        System.out.println("Encrypted_message"+encrypted_message                    );
        System.out.println("Decrypted_message_before_removing_boggus"+decrypt_message_boggus);
        System.out.println("Decrypted message"+decrypted_message);
    }
}

