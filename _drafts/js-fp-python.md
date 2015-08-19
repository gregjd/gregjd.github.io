---
layout: post
title:  "How JavaScript and functional programming have influenced my Python"
categories: jekyll update
---





Yet over the course of the three introductory computer science courses I took, we never covered these topics.
They're so powerful! I wish they were more widely taught.



>> (Both) Made me more comfortable using first-class, higher-order, inner, and anonymous functions

Assigning functions as the values of variables, using functions as parameters ____example____

Python lambdas

Returning functions (include elsewhere, like in the closures/currying section?)

>> (FP) Thinking more in terms of map, filter, and reduce, and less in terms of loops

In the classic imperative vs. declarative

When it comes to "taking a list of something and doing something with it," we can either describe the mechanics of what we want to do or describe what we want done. Loops accomplish the former, while map/filter/reduce (and other related functions) accomplish the latter.

I've found that it can be a lot more intuitive to describe operations in declarative terms
What I really like is that you're focusing more on describing the goal rather than the strategy, leading you to reason more carefully about what you're actually doing.

Of course, sometimes it's easier and quicker to just write a for loop. So assuming I'm using a language like Python or JavaScript, I do.


>> (Both) Inspired me to make use of closures and currying

___examples___


Closure

```python
def addPropFromJSON(file_name):

    f = open(file_name, 'r')
    js = json.loads(f.read())
    f.close()

    def jsonMatch(lookup):

        try:
            return js[lookup].encode('ascii')
        except KeyError:
            print lookup, 'not found in JSON file'
            return None

    return jsonMatch
```

In this case, we given a JSON file name as input and get a function as output. Our output function has access to the contents of the JSON file (js); this way, we only have to open the file once rather than needing to open it each time we want to look something up. Our jsonMatch function has access to.


>> (FP) Helped me reason better about inputs, outputs, and side effects

Two of the most important aspects of pure functional programming are that functions don't make use of "hidden inputs" (meaning, relying on external state) and that functions don't have any "output" besides their return values (meaning no side effects). Thus, a given set of parameters always produces the same output, and functions are equivalent to what they evaluate to (referential transparency).

All of this is a big deal because it's not just useful for functional programming, it also helps you (me) write better imperative code. I make sure that functions rely soley on their explicit inputs, rather than calling global variables. And when commenting my functions, I explicitly state any side effects, in addition to listing arguments and the output.

Sometimes, you do need side effects (thus breaking referential transparency) --- in fact, sometimes side effects are the point of a function --- but thinking in functional terms can still help you better describe those effects and be careful to limit them.


>> (FP) Encouraged me to write smaller functions and more modular code

Smaller functions are great for many reasons:
* They promote reuse, modularity, and separation of concerns
* They are easier to reason about (i.e. seeing that a given set of inputs will produce a certain output)
* They are easier to test
* They are more readable, as it's usually more clear what their purpose is

Functional programming has very much encouraged me to write smaller functions and combine them, rather than having large functions that do lots of things.


>> (Both) Made me rely on object-oriented programming less

Clearly FP

I remember when I was first learning about JSON, I noticed that these things that were being called "objects" looked exactly like what would be dicts in Python. Later, of course, I learned why JSON calls them objects --- because they literally are objects in JavaScript (thanks to first-class functions being used to create an object's methods), with one data structre being used for what are two different concepts (objects and dicts) in Python. This made me think about both objects and hash tables in a new way. In particular, it made me realize that some uses of objects (in languages like Python) are quite silly, as they are so simple that they could easily be replaced with dicts. (Granted, if you go JavaScript-style, any object could be replaced with a dict.) For example, I looked at a past project of mine where the primary purpose of objects was to hold instance variables and accessor methods, and realized these could just be dicts whose values I reference.

>> (JS) Made me more inclined to use dict literals

Since JavaScript's objects are basic

Using functions as values (or include in the first-class functions section?)

