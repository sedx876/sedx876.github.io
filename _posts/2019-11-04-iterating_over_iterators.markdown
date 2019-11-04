---
layout: post
title:      "Iterating over Iterators"
date:       2019-11-04 23:12:04 +0000
permalink:  iterating_over_iterators
---


**Iterate** [ it-uh-reyt ]
verb (used without object), it·er·at·ed, it·er·at·ing.
to operate or be applied repeatedly, as a linguistic rule or mathematical formula.

**Ruby Iterators**-  is the object-oriented concept in Ruby. In more simple words, iterators are the methods which are supported by collections(Arrays, Hashes etc.). Collections are the objects which store a group of data members. Ruby iterators return all the elements of a collection one after another. A Ruby iterator is simply a method that can invoke a block of code. 

Iterators are a basic but helpful tool in Ruby. Without them we would not have basic functionalities that are needed in programming. Iterators can be chained together to get even more specific returns.

There are a few ways to accomplish iteration and get back the data we are looking for.

**.each**- This will return all elements in a hash or an array. But it does not change the return value. It implicitly returns the original collection. There are variances of **.each** such as: **.each_with_index** and **.reverse_each**

**.map/.collect**- These two iterators basically do the same task. Map and Collect differ from **.each** such as it returns a new array of values

**.select**- This will return values that it iterates over only if the value is found to be true by the parameters we give. **.detect** works in a similar fashion.

**.find**- This will return the first value that satisfy the parameters that are given in the code and stops there.

**.find_all**- Will return all the values that satisfy the parameters that are given.

**.times**- This iterator is used to iterate through the array from 0 to n-1 index position.

There are even more iterators than listed here. The ones discussed here are the more commonly used ones. Iterators help make your code cleaner and simpler to work with. If you have a collection of elements that needs to be analyzed or manipulated in a certain way there is probably an iterator just waiting to be implemented.
