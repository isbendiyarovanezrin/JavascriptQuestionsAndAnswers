<div align="center">
  <img width="50" src="https://i.postimg.cc/h4dzTwG8/javascript.png">

### **JavaScript Interview Questions and Answers**

</div>
<br>

1. #### **What is the difference between == and === operators?**

   "==" operatoruna bərabərlik operatoru deyilir. Dəyişənlərin data tiplərini nəzərə almadan iki dəyişəni müqayisə etmək üçün istifadə edilir və boolean dəyər (true və ya false) qaytarır. Əgər dəyişənlərin dəyəri eynidirsə true qaytarır, deyilsə false qaytarır. <br>
   "===" operatoruna isə qatı bərabərlik operatoru deyilir və "==" operatorundan fərqli olaraq iki dəyişənin həm dəyərini müqayisə edir, həm də data tiplərini yoxlayır. Əgər hər ikisi də eynidirsə true qaytarır, deyilsə false qaytarır. <br>

   _Bir neçə nümunəyə baxaq:_

   ```js
   "you" == "you"; // true
   "you" === "you"; // true
   "your" === "you"; // false
   5 == "5"; // true
   5 === "5"; // false
   5 == 5; // true
   5 === 5; // true
   0 == false; // true
   0 === false; // false
   1 == true; // true
   1 === true; // false
   null == null; // true
   null === null; // true
   null == undefined; // true
   null === undefined; // false
   NaN === NaN; // false
   ```

<br>

2. #### **What is null value?**

   Null dəyərin yoxluğunu ifadə edən JavaScriptə xas primitiv data növüdür və typeof operatorundan istifadə edəndə object qaytarır. <br>

   _Nümunə:_

   ```js
   let test = null;
   alert(test); // null
   alert(typeof test); // object
   ```

<br>

3. #### **What is undefined property?**

   Undefined dəyişənin olduğunu, lakin dəyər təyin edilmədiyini bildirən primitiv data növüdür və typeof operatorundan istifadə edəndə undefined qaytarır. <br>

   _Nümunə:_

   ```js
   let test;
   alert(test); // undefined
   alert(typeof test); // undefined
   ```

<br>

4. #### **What is isNaN?**

   JavaScriptdə isNaN() metodu dəyərin rəqəm olub-olmamasını yoxlayır və boolean dəyər (true və ya false) qaytarır. Əgər dəyər NaN (**N**ot **a** **N**umber) olarsa (yəni rəqəm olmazsa), bu zaman true qaytarır, əks halda false qaytarır. <br>

   _Nümunə:_

   ```js
   isNaN(20); // false
   isNaN("20"); // false
   isNaN("20.55"); // false
   isNaN("20,55"); // true
   isNaN("text"); // true
   isNaN(""); // false
   isNaN(" "); // false
   isNaN(null); // false
   isNaN(undefined); // true
   isNaN(NaN); // true
   isNaN(true); // false
   isNaN({}); // true
   isNaN(new Date()); // false
   ```

<br>

5. #### **What is the typeof operator?**

   JavaScriptdə typeof operatorundan dəyişənlərin data tipini tapmaq üçün istifadə olunur. <br>

   _Nümunə:_

   ```js
   // numbers
   typeof 55; // 'number'
   typeof 55.12; // 'number'
   typeof Infinity; // 'number'
   typeof NaN; // 'number'
   typeof Number("5"); // 'number'
   typeof Number("paper"); // 'number'

   typeof 55n; // 'bigint'

   // strings
   typeof ""; // 'string'
   typeof "3"; // 'string'
   typeof "text"; // 'string'
   typeof `string text`; // 'string'
   typeof typeof 5; // 'string'

   // booleans
   typeof true; // 'boolean'
   typeof false; // 'boolean'

   // undefined
   typeof undefined; // 'undefined'

   // objects
   typeof null; // 'object'
   typeof { name: "Samir" }; // 'object'
   typeof [5, 55, 12]; // 'object'
   typeof new Date(); // 'object'

   // function
   typeof function () {}; // 'function'
   ```
