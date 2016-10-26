# call and apply

 > The call() method calls a function with a given this value and arguments provided individually.
 
 > While the syntax of this function is almost identical to that of apply(), the fundamental difference is that call() accepts an argument list, while apply() accepts a single array of arguments.
 
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
