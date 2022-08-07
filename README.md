ANONYMOUS or IIFE functions

Print odd numbers in an array:

function(array){
                  for(var i = 0 ; i< array.length ; i++){
                        if(array[i]%2!=0){
                           console.log(array[i])
                        } 
                   }
                }

Convert string to title case :

 function (str) {
                    str = str.toLowerCase().split(' ');
                    for (var i = 0; i < str.length; i++) {
                      str[i] = str[i].charAt(0).toUpperCase() + str[i].slice(1); 
                    } 
                    return str.join(' ');
                  }

Sum of all numbers in an array :

function(array){
                  var sum = 0;
                  for(var i = 0 ; i< array.length ; i++){
                     sum = sum + array[i];
                   }
                   return sum;
                }

Return all the prime numbers in an array :
   
              function(numArray){
                  numArray = numArray.filter((number) => {
                    for (var i = 2; i <= Math.sqrt(number); i++) {
                      if (number % i === 0) return false;
                      }
                      return true;
                     });
                    console.log(numArray);
                    
 Return all the palindromes in an array :                   
                    
  function isPalindrome(S)
    {
        let str = "" + S;
        let len = str.length;
        for (let i = 0; i < +(len / 2, 10); i++)
        {
            if (str[i] != str[len - 1 - i ])
                return false;
        }
        return true;
    }    
  
  
  Rotate an array K times :
    
    function(array , k){
                          k = k % a.length;
                            if(k < 0){
                              k += a.length;
                            }

                            reverse(a, 0, a.length - k - 1);
                            reverse(a, a.length - k, a.length - 1);
                            reverse(a, 0, a.length - 1);
                          }



USING ARROW FUNCTIONS :

Print odd numbers in a array :

oddNumbers = (array) => {
                   for(var i = 0 ; i< array.length ; i++){
                        if(array[i]%2!=0){
                           console.log(array[i])
                        } 
                   }
                        }
                        
                        
Convert string to title case :                      
                        
              titleCase = (str) => {
                    str = str.toLowerCase().split(' ');
                    for (var i = 0; i < str.length; i++) {
                      str[i] = str[i].charAt(0).toUpperCase() + str[i].slice(1); 
                    } 
                    return str.join(' ');
                  } 
                  
Sum of all numbers in an array :                
                  
              sum = (array)=>{
             var sum = 0;
                  for(var i = 0 ; i< array.length ; i++){
                     sum = sum + array[i];
                   }
                   return sum;
                   }  
                   
All prime numbers in an array :                 
                   
primeNumber = (numArray) => {
                      numArray = numArray.filter((number) => {
                        for (var i = 2; i <= Math.sqrt(number); i++) {
                          if (number % i === 0) return false;
                        }
                        return true;
                      });
                      console.log(numArray);
                  }
