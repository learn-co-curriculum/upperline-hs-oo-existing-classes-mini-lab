

# Re-Opening Existing Classes Mini-Lab

Recall from our lecture that everything in Ruby is an object, and every object has to come from a class. For example, an integer (like `5`) comes from the `Integer` class, and we can create new integers like so:
```ruby
x = Integer.new(3)
```

We can re-open classes to add more methods. Here I'm going to add a `square` method to the integer class that will give me the square of the integer instance.

```
class Integer
  def square
    self * self
  end
end
```
I can test it out here:
```
3.square #=> 9
```

`self` in this situation is the instance of the object itself. [Here's some more reading on `self`](http://www.jimmycuadra.com/posts/self-in-ruby).

## Your Challenge

Here are a few additions to existing classes that you should try:

+ Add a method `.exclaim` to the `String` class that returns "OMG! ______ OMG!" (the blanks space should be replaced by the original string).

+ Add a method `.zizzify` to the `String` class that converts all 's's in a string to 'z's

+ Add a method `.is_a_square?` to the `Integer` class that returns true if the integer is a square number (1,4,9, etc), and false otherwise.

+ Add a method '.third_item' to the `Array` class that returns the third item in an array. If there is no third item, it should return the string "Womp, womp."

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/hs-oo-existing-classes-mini-lab' title='Re-Opening Existing Classes Mini-Lab'>Re-Opening Existing Classes Mini-Lab</a> on Learn.co and start learning to code for free.</p>
