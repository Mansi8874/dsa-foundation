Print all subsequences of a string

// Java program for the approach

Given a string, we have to find out all subsequences of it. A String is a subsequence of a given String, that is generated by deleting some character of a given string without changing its order.

Examples: 

Input : abc
Output : a, b, c, ab, bc, ac, abc

Input : aaa
Output : a, a, a, aa, aa, aa, aaa

# Algorithm

The concept of subsequence either character will present or not.

In main function firstly we created the string and then we have called the subsequence function which will print the subsequence of string.

The subsequence function will take the String ,index and newstring and when we will reach the base case it will print the newstring and return.

        <!-- if(idx==str.length()){
            System.out.println(newString);
            return;
        } -->

There will be two option either the character will come or it will not come so we call recursion one by taking the currchar and second without taking character.

        <!-- char currchar=str.charAt(idx);

        // when we consider the currchar
        // We add adding 1st character in string
        subsequence(str, idx+1, newString+currchar);

        // when we did not consider the currchar
        // Not adding first character of the string
        // because the concept of subsequence either
        // character will present or not
        subsequence(str, idx+1, newString); -->

Time Complexity : O(2^n) where n is length of string

