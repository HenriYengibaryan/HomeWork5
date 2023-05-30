# HomeWork5
/1 1. Write a function to determine if number prime.


function num(x){ 
    let count=0
        x=Math.abs(x)
        for(let i = 1; i<=x;i++){
            if(x/i===Math.round(x/i)){
                count++
            }
        } if(count>2){
            return false
            
        } else if(x===0){
            return 'voch parz voch baxadryal'
        }else{
            return true
        }
    
    return
    }

    
    
//2 2. Write a function to console.log all prime numbers before the given number.
  

  function isPrime(x){ 
        let count=0
            x=Math.abs(x)
            for(let i = 1; i<=x;i++){
                if(x/i===Math.round(x/i)){
                    count++
                }
            } if(count>2){
                return false
                
            } else if(x===0){
                    return false
            }else{
                return true
            }
        
        return
        }
    function logPrime(x) {
        for(let i =0;i<=x;i++){
            if(isPrime(i)){
                console.log(i)
            }
        }
    }


    // 3 Write a function, which receives a string, finds possible largest numbers in the string and
// returns their sum.
  

  function string(x) { 
        let count = 0
        let str =''
        for(let i =0;i<x.length+1;i++){
            if(+x[i]===Math.abs(x[i])){
                str+=x[i]
            } else{
                count+= +str
                str=''
            }
        }
    return count
}
    

//4 4. Write a function which receives two strings and removes appearances of the second
    //   string from the first one.
   

 function text(x,y) {     
        let str =''
let twoCharacter=y
for(let i=0;i<x.length - 1;i++){
if(x[i]===' '){
i++
str= str+' '
}
let twocharact1=x[i]+x[i+1]

if(twocharact1===twoCharacter){
i++
}else{
str+=twocharact1
i++
}
}   

return str
}




//55. Write a function to compute a new string from the given one by moving the first char to
//come after the next two chars, so &quot;abc&quot; yields &quot;bca&quot;. Repeat this process for each
//subsequent group of 3 chars. Ignore any group of fewer than 3 chars at the end.
  




function simbol(x) { 
    let threeChar=''
    let change=''
    if(x.length>=3){
        for(let i =0; i<x.length-1;i++){
            if(i+2<=x.length-1){
        threeChar+=x[i+1]
        threeChar+=x[i+2]
        threeChar+=x[i]
            change+=threeChar
            threeChar=''
            i+=2
            } else if((i+1)===x.length-1){
                threeChar+=x[i]
                threeChar+=x[i+1]
                change+=threeChar
                st=''
            }else if(i===x.length-1){
                threeChar+=x[i]
                change+=threeChar
            }
                
            
     } 
    } return change
}
