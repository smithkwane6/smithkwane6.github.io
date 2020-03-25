---
layout: post
title:      "SIMPLE AS I CAN PUT IT"
date:       2020-03-25 04:10:35 +0000
permalink:  simple_as_i_can_put_it
---


Using one of the easier labs given in iteration, the square array lab, I will make a strong attempt at teaching someone how to solve and code this lab.  This objective of the square array lab is very self-explanatory. If knowledge of what an array is and how we will iterate over each item in the array. In this case we’ll be writing code that should take each number in an array and square that number to create a new array with the results of those squared items in the previous array.

Like I mentioned earlier in order to get through this lab there should be some research or studying done about what exactly an array is. According to Google, when it comes to ruby, arrays are ordered, integer-indexed collections of any object, which can hold objects such as string, integer, fixnum, hash, symbol, even other array objects.  Normally arrays are identified with the “[]” blocked like braces, with each item inside separated by a comma.  Also, it would help to understand that with iteration, every item in said array will have something done with it.  Using iterators such as “each” and/or “do”, both yields each element one at a time to every iteration via a variable declared with the opening of a block.  Google is the perfect way to find the endless amount of detailed information about iterators and how they work.

Getting to the square array lab, the read me states that the objectives are that we want to practice iterating over an array using the “. each” method. Along with practice operating on each element of an array.  Basically, the instructions state that we want to build a method, square_array, that squares each element in an array of numbers and returns a new array of these squared numbers. Which is fun because we learn how to properly use “. push” also while coding this lab.  The read me for this lab also gives a few questions that will help if you ask yourself while working on this.  One being what is the return value of calling “. each” on an array, or how can we operate on each element of an array and collect or store those elements. Both of which will be answered by using those iterators mentioned earlier, along with another “. collect”.  

First things first like the read me stated we want to define our method square_array.  I did so by using this bit of code.

	def square_array(array)
	#code here
	end
	
As you can see, I defined the method square_array and pushed in the argument of array and ended it like any other defined method with an end.  Next, we want to figure out what code we can use that will achieve what we want to do with our array.  With this lab an array isn’t given, so what I want to do is create a new array.

	def square_array(array)
	 	new_array = [ ]
	end
	
Simply put I created an array by naming it new_array and setting it equal to what is known as an empty array identified by the [ ] block like braces.  Next, I know that I want my code to iterate over each item in that array.  Here I get to use the “. each” and “do” iterators mentioned earlier as such.

	def square_array(array)
		new_array = [ ]
		array.each do |x|
	end 
	
From here I want to tell my block what is basically expected. I want to square an array of numbers and push those results into a new array.  And then, call upon that new array so that we may use it.  I achieved this using the following code.

	def square_array(array)
		new_array = [ ]
		array.each do |x|
		         new_array.push x*x	
	end 

	new_array
	
	end

At this point, should be able to give a set of numbers in an array, and with the code created, be able to get the squared result of those numbers.  With those results given in a array of their own.  I’m sure there are many million other ways to achieve the same thing, but this is the way I went about it. The code is simple, concise, and gets the job done.


