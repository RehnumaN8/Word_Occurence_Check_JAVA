# Word_Occurence_Check_JAVA
Write a Java program that reads a text file and counts the occurrences of each word in the file. The program should then display the word count for each unique word in alphabetical order.

The Code is given below:

----------------------------------!!!!!!!!!-----------------------------------------------------------------------

import java.util.*;
class StringWordCountOccurence
{
    public static void main(String[] args)
    {
        String s= "The quick brown fox jumps over the lazy dog. The lazy dog slept.";
        
        String arr[]=s.split(" ");
        int count=0;
        Map <String,Integer>map=new TreeMap<>();
        for (int i=0;i<arr.length;i++){
            count=0;
              for(int j=0;j<arr.length;j++){
                  if(arr[i].equals(arr[j])){
                      count++;
                  }
              }
              map.put(arr[i],count);
        }
        System.out.println(map);
    }
}




