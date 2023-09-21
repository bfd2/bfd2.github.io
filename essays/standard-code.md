---
layout: essay
type: essay
title: "Standardized Coding"
# All dates must be YYYY-MM-DD format!
date: 2023-09-21
published: true
labels:
  - Coding Style
  - Standards
---
![](https://cdn.sketchbubble.com/pub/media/catalog/product/optimized1/4/1/4157b6f345d365b0b5318f39e3d102a183dd0c0c53237441e99e7221b3a914fb/coding-best-practices-mc-slide3.png)
## The Standards of Coding

----

Coding standards is a big topic and there are a lot of different standards that people abide by in the Computer Science industry. Personally, coding standards are a good thing since they can help code readability and make code a lot more better. But the standards need to make sense and actually be useful to other people. One of the worst standards that I have to follow for one of my computer science classes is using constants for everything, meaning that if you wanted to change a value of a variable, you’d have to create another constant variable and then manipulate the value of the variable that you want to change. It frustrated me a lot and I learned nothing of value from that class.

## A Good Standard

----
Good standards help create good habits which translates into good coding. One of the most helpful standards I learned is putting your curly brackets on new lines. I know for some people it is a waste of space but it is very useful if you are writing functions that contain a lot of nested loops that can be confusing to dissect if they are all cramped into one line of code. Would you rather read this:
```angular2html
while(this != true){if(p == 1){return 0;}else if(p == 2){for (int i = 0; i < a.length; i++){ j = j + 2 }}else {break;}
```
or this: 
```angular2html
while (this != true)
{
    if (p == 1)
    {
        return 0;
    }
    else if (p == 2)
    {
        for (int i = 0; i < a.length; i++)
        { 
            j = j + 2 
        }
    }
    else 
    {
        break;
    }
}
```

It is more helpful to see the structure and scope of the code if it is more spaced out (although it may look ugly and daunting to some people.) But there's so much room for the code to breathe and makes it easy on your eyes instead of the claustrophobic and dense feeling that you get from a somewhat obfuscated one-liner. I rather take the readability of the code than the convince of having it crammed into one line for simplicity and "just cause it's cool." 

## Documentation

----
Above all, I think the most important coding standard that everyone should follow is documenting and commenting on your code. I think this should be a universal rule if it isn't already. If you don't document your code, then you're either evil or just like being confused. You want everyone, include yourself, to know what the code does and what everything does down to the tee. You want even someone from 100 years in the future to know what your code does instead of them wasting time testing and debugging what your code does. But the best tip is to make sure your comments make sense. Don't do this:
```angular2html
// adds to array
function c (a[], int b) {...}
```
Be more detailed. Explain and make it concise.
```angular2html
// appends integer b to the array a. Returns the array a.
function c (a[], int b) {...}
```
It's a simple trick that can go a long way. It's also the reason why open source programming is one of the best parts of programming since it allows anyone to edit the code and make the project a lot better than if it were only done by a secluded group of individuals. Then again, I could've name my function appendToArray to make it more obvious. 

If you don't document your code, then what's the point of coding in the first place?

## Lint and Rollers

----
Some people may find coding analysis tools like ESLint useless because it forces you to conform to a standard that can be annoying to deal with. 

But think about this.

Imagine a team of 10 people, all with varying coding styles that have their own way of naming conventions, variable declarations, documenting, and how they structure their code. It would be very annoying to try and figure out whose code does what, pinging them on Discord late at night to ask what their functions do, and trying to debug it because another person's functions messes with their functions, and so on.

But now that we have one standard from ESLint, everyone's code is the same structure and conventions, which saves time on reading and debugging. It also catches unused variables and console logs that you might not catch because you slept 2 hours in the past week. You can also config ESLint to your liking but personally leaving it on the default settings is good enough since almost everyone knows what the standard is. 

<img src="https://eslint.org/assets/images/eslint-features-img-600w.jpeg" alt="drawing" width="600"/>

(I mean, look how beautiful this code looks, beside the error squiggly of the Collection. I just took this from the official ESLint project site.)

## No Stake in Courtesy

----
Finally, the best standard that I think everyone should follow while coding is using common sense. Always ask yourself: "Can a 9 year old kid know what my code is doing just from reading it?" If not, start commenting and making it more concise and readable. Unless you're creating code for a CTF competition and obfuscating JavaScript and assembly, the more readable the code, the more eyes that can help and improve your code. The best things in life are always short and sweet. Good code creates good habits, which can lead to a greater lifestyle. Use good standards like AirBNB and your code will look amazing.