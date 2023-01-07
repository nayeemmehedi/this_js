# this_js

this

first rules

this child r parent  object k bujhai 
parent r vtr j ase child access pabe



rules 2 
this always function e kaj kore - function 
r upore tar parents object thkte hy



   const parents ={
    myChildName : "Mew",

    thisCheck : function(){
        console.log(this.myChildName)
     }

   }

     parents.thisCheck()

rule3 

function r vtr function thke this kaj krbe na value pabe na 



    const obj = {
        name: "nayeem",

        methodName: function () {
           
            console.log(this.name) //nayeem
            function boom() {
                console.log(this.name) //undefined
            }
            boom()
        }
    }

    obj.methodName()


rules 4 

()=> arrow function r kono this nai nijsso so o eshb bujhe na parent function r this thkle o seta pabe nyto pabenna.
jdi obj parent hy thle this pabe na


subrule 1

parent r this.name  r value nai methodname e , so boom o this.name nai


    const obj = {
    name: "nayeem",

    methodName:  () =>{
   
        console.log(this.name) //undefined
        const boom=()=> {
            console.log(this.name) //undefined
        }
        boom()
      }
    }

     obj.methodName()


subrule 2

parent r this.name  r value ase methodname e , so boom o this.name pyse 

    const obj = {
    name: "nayeem",

     methodName:  function(){
   
        console.log(this.name) //nayeem
        const boom=()=> {
            console.log(this.name) //nayeem
        }
        boom()
     }
    }

    obj.methodName()




