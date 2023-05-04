Download Link: https://assignmentchef.com/product/solved-cs52-assignment-5-oop-inheritance
<br>
<strong>Shopping Cart                                 </strong>

Implement a program that tracks customers’ purchases. Create the following classes. Use appropriate access modifiers (instance variables should be private!) and data types for each. Don’t forget to add getter and setter functions.

<ul>

 <li><strong>Item</strong>: This      class     has        the        attributes         (member              variables)          called   title,     description,     and

  <ul>

   <li><strong>Book</strong>: This      class     inherits              from         It              has        an         instance            variable              called   pageCount.      o <strong>Movie</strong>:           This              class     inherits              from     Item.    It              has        an         instance            variable              called   length.</li>

   <li><strong>CD</strong>: This      class     inherits              from         It              has        an         instance            variable              called   trackCount.</li>

  </ul></li>

 <li><strong>ShoppingCart</strong>: This class     keeps   track     of          items              that      were                  You       may      limit              the        number             of          items    in           the              cart.      The       cart       should have     functions          to              add       an         item     and       print     the        items              currently           in           the        cart       to          the              console.</li>

 <li><strong>Customer</strong>: The       customer          class     stores   an         id,              the        first       name   and       the        last       name              and       a            pointer to          a            shopping              cart</li>

</ul>

Finally, implement a main function that creates a customer. Then add one item of each type to the customer’s shopping cart and list the items in the cart on the console.

<strong>Problem 2</strong>                                           <strong>Pizza                                                </strong>

Implement a program that creates pizzas based on user order. First, create class called <strong>Ingredient</strong> with one instance variable <em>description</em> of type <em>string </em>which is set in the constructor and can be get using a getter function. Create the following classes that derive from Ingredient: <strong>TomatoSauce</strong>, <strong>Cheese</strong>, <strong>Dough</strong>, and <strong>Pepperoni</strong>; each with a constructor that passes the <em>description</em> argument to the base constructor. Use proper access modifiers!

Programming

Create a class <strong>Pizza</strong> which consists of a dynamically allocated array of Ingredient object pointers (a double pointer). The constructor expects the number of maximum ingredients as <em>int </em>which is used to dynamically allocate and initialize the array. Implement a destructor that deletes the Ingredient objects and the array. The class has a function <em>void add(Ingredient* ingredient)</em> which adds an ingredient to the pizza and a function to print its ingredients to the console.

Create an abstract class <strong>PizzaFactory</strong> with a <u>pure virtual function</u> called <em>bake()</em> that returns a

<em>Pizza*</em> object pointer. Create the two subclasses <strong>CheesePizzaFactory</strong> and

<strong>PepperoniPizzaFactory</strong> which both explicitly override the <em>bake()</em> function. Both functions should remain <em>virtual</em>. The <em>CheesePizzaFactory</em> instantiates Pizza and adds Dough, TomatoSauce, and Cheese to it. The <em>PepperoniPizzaFactory</em> creates a pizza and adds all ingredients including pepperoni to it.

Use the following main method which prompts a user to order a type of pizza and then instantiates the corresponding PizzaFactory for it. After the pizza is created by calling the <em>bake()</em> function, the ingredients of the pizza are printed by calling the <em>listIngredients()</em> function of the pizza object. Finally, the factory and the pizza objects are deleted.