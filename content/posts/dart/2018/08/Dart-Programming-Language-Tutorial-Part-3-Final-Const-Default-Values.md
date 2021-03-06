---
title: "Dart Programming Language Tutorial Part 3 | Final,Const, and Default Values"
description: "In the last post we looked into how to declare and print variables. In this post we will conclude the section on variables by discussing about final and const keywords and default values"
author: "Rishabh Jain"
keywords: ["rishabh","rishabh jain","rishabh1403","blog","dart","dartlang","variables","final","const","default","values","tutorial","programming","language"]
tags: ["dart","tutorial"]
categories: ["dart"]
date: 2018-08-29T21:45:47+05:30
draft: false
---
In the last post we looked into how to declare and print variables. In this post we will conclude the section on variables by discussing about final and const keywords and default values.
<!--more-->
# What's the need of a constant ?
Variable as the name suggests varies over time, i.e. the value it holds changes. However sometimes we don't want values that a variable holds to change over the course of a program. Let's say we are storing the value of `pi` in our code to do some calculations. Now we don't want someone to change the value that our `pi` variable is storing by mistake. In that case we need to take some measures to make sure no one changes the value of these variables or more correctly `constants`. We can declare a constatnt using either `final` or `const` keyword.

# Final and Const

The syntax to declare a variable final or const is very simple. Let's see some code snippets below.

```dart
    void main(){
        // code starts here
        
        final a = 3;
        final int b = 3;

        const c = 3;
        const int d = 3;
        // code ends here    
    }
```

In the code snippet above we make two final `declarations` and two const `declarations`.
Points to note with these declarations are

* We have used either `final` or `const` keyword to declare a variable final or constant
* We cannot use `var` along with `final` or `const`
* However we can annotate with specific data type if we want to

If you really think about it, dynamic declaration doesn't make sense here, because we aren't allowed to change data anyway. So these are the key points to note in `final` and `const`. The moment you declare a variable final or const, you cannot change it afterwards. If you try to assign another value to the variable later on, it will throw an error. You must be thinking, what is the difference between `final` and `const`. Both looks pretty much same. Actually in case of variables, yes they are, but they have some differences which we will look into while dealing with classes. Actaully final creates constants variables while const creates constant values. More on this in classes section.

# Default Values

Default values are the values that get assigned to a variable when you declare them but don't initialize them. If you are coming from golang background it is very similar to `zero values`. However in dart, the default value for all types are `null`. 

```dart

    void main(){
        // code starts here

        var a;
        
        assert(a==null)

        // code ends here
    }
```

In the above code snippet, I declared a variable `a`, but didn't assign any value to it. Dart by default assigns `null` to it while declaration. In the next line we are just proving that `a` is null. If that was not the case, the `assert` statement would have thrown an error. That's it for this one guys, with this we have concluded our variables section. In the next one we will start with something new and more exciting. 

There you go guys, you made it to the end of the blog. Please check out the video below if you still have any doubts, subscribe to my [youtube channel](https://www.youtube.com/channel/UC4syrEYE9_fzeVBajZIyHlA) for regular updates, subscribe to my mailing list below, follow me on [twitter](https://www.twitter.com/rishabhjain1403) , drop me a mail or leave a comment here if you still have any doubts and I will try my best to help you out. Thanks

Stay tuned and see you around :)
{{< youtube syqItkjNYHo >}}  
