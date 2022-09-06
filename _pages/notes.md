---
layout: page
title: Notes
permalink: /notes/
---


Front matter - Section at the top of your jupyter notebooks that helps to manage fast pages

![]({{ site.baseurl }}/images/frontmatter.png "front matter example")

Primitive Java Data Types
- boolean
- char
- byte
- short
- int 
- long
- float
- double

Non-Primitive Java Data Types
- String
- Array
- class
__________________________________________________________________________

- Constructors: methods with the same name as the class it is in. It is a speacial methods used to initialize objects. Here is a constructor that takes parameters inside of a class called ThreeString - [Exploration Code](https://tangalice.github.io/alicetang/java/jupyter/2022/09/04/ThreeString.html)
```
//constructor that takes parameters
   ThreeString(String str1, String str2, String str3)
   {
      if (validString(str1) && validString(str2) && validString(str3))
      {
         string1 = str1;
         string2 = str2;
         string3 = str3;
      }
      else
      {
         string1 = DEFAULT_STRING;
         string2 = DEFAULT_STRING;
         string3 = DEFAULT_STRING;         
      }
   }
```

- Mutators: methods that mutate the value of a private member variable. Here the methods setString1 sets the value of a private member of the ThreeString class called string1
```
public boolean setString1(String str) 
   {
      boolean status = false;
      if (validString(str))
      {
         string1 = str;
         status = true;
      }
      return status;
   }
```

- Accessors: methods that accesses and returns the value of a private member variable. Here the getString1 method acesses and returns the value of the private member string1.
```
 public String getString1()
   {
      return string1;
   }
```


