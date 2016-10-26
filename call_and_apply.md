# call and apply

 > The call() method calls a function with a given this value and arguments provided individually.
 
 > While the syntax of this function is almost identical to that of apply(), the fundamental difference is that call() accepts an argument list, while apply() accepts a single array of arguments.
 
*<small>翻译：call方法调用函数时，提供单独的值和参数。<small>*

*<small>翻译：而call语法几乎和apply相同，根本的区别是call接受一个连续参数列表，而apply接受一个数组参数。<small>*

### Syntax

 > fun.call(thisArg[, arg1[, arg2[, ...]]])
 
 > fun.apply(thisArg, [argsArray])
 
### example

1.第一个参数是任一个对象，没有区别。

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
  blackCat.say.call(dog);  // I love bone
  blackCat.say.apply(dog)  // I love bone
  ```
  
2.多个参数时。
  
  ```html
  function add(j, k){
    return j+k;
  }

  function sub(j, k){
      return j-k;
  }
  
  add(5,3); //8
  add.call(sub, 5, 3); //8
  add.apply(sub, [5, 3]); //8

  sub(5, 3); //2
  sub.call(add, 5, 3); //2
  sub.apply(add, [5, 3]); //2
  ```
  
3.对象的继承。

  ```html
  var Parent = function(){
      this.name = "yjc";
      this.age = 22;
  }

  var child = {};
  console.log(child);  // Object {}

  Parent.call(child);
  console.log(child);   // Object {name: "yjc", age: 22}

  ```
  
  
