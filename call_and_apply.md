# call and apply

 > The call() method calls a function with a given this value and arguments provided individually.
 
 > While the syntax of this function is almost identical to that of apply(), the fundamental difference is that call() accepts an argument list, while apply() accepts a single array of arguments.
 
*<small>翻译：call方法调用函数时，提供单独的值和参数。<small>*

*<small>翻译：而call语法几乎和apply相同，根本的区别是call接受一个参数列表，而apply接受一个数组参数。<small>*

### Syntax

 > fun.call(thisArg[, arg1[, arg2[, ...]]])
 
 > fun.apply(thisArg, [argsArray])
 
### example

  ```html
  function cat(){

  }
  cat.prototype={
    food:"fish",
    say: function(){
    console.log("I love "+this.food);
    } 
  }
  
  var blackCat = new cat;
  blackCat.say();
  // I love fish
  
  var dog = {food:"bone"}
  blackCat.say.call(dog);
  blackCat.say.apply(dog)
  // I love bone
  // I love bone
  ```
