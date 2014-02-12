grunt-supersass
===============

More than just a sass compiler. A SaSS workflow.


# Reasons. 

I use the term SaSS to mean both SaSS and CSS.

## SaSS belongs next to the html that uses it 
This way : 
* If you delete some html you know which sass is redundant (orphaned).
* Super simple to find SaSS associated with the HTML. 


## Html should have its own classes per html file
It is very difficult to come up with Highly generic across the board consistent sass classes. 
You can find a common ground but there is always some customization required here and there. 

So the workflow is to have these Common SaSS classes in one place. 
And then in each HTML's SaSS @extend these. 

Addtional Advantage: Can you tell me all the places that will be impacted if you modify 
your definition of `span6`. Probably not. I can. I just search for all the instances of `span6` in my sass
since I don't use it in my html. 
