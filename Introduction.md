# Introduction
This is a series, where I'll post what I've learn about JSON on GitHub. Publishing this on the git so that I can revise, as well as help anyone who wants to learn JSON themselves. Since my primary language is Python and I am learning JSON to use it along with Python, All chapters would focus on JSON and its integration with Python and its data types. 

# Introduction to JSON


1. JSON stands for JavaScript Object Notation, it is inspired by JavaScript. It is mainly used to store and exchange structured data between different programming languages. 
2. As the name suggests it is inspired by JavaScript, but it is language independent.
3. It is compatible with most of the languages, like in Python it uses dictionaries to represent JSON objects and lists to represent JSON arrays. Python's JSON library can convert JSON data into corresponding Python data types and vice versa.
4. It is widely used in web applications, particularly for exchanging information between clients and servers through APIs. 

# When to use JSON and why?
1. Useful in storing data in human readable format.
2. Communication between applications, for e.g. in a web application, the website might need to retrieve data from an external service, so it can send the request containing JSON data, as it is lightweight, human-readable as well as easy to convert in other languages.
for eg: 
    Let's say in simple weather app, you want to know about the weather of a particular place. Since the website doesn't have access to real-time weather data, it needs to communicate with an external weather service(API). But how would then the problem arises that how would we send the information to the server for retrieval? 
    So that is done using JSON, XML, etc. So website would send something like this: 
    {
        "city" : "Mumbai"
    }
    Here, *city* is the key, and *Mumbai* is its corresponding value. The weather service processes this request and retrieves the relevant weather information for Mumbai. 
    And would return data as: 
    {
        "city": "Mumbai",
        "temperature" : 29,
        "humidity" : 80,
        "weather" : "Cloudy"
    }
3. JSON can also store an application's settings and configurations.
    for eg: 
        {
            "theme" : "dark",
            "notifications" : true,
            "Language": "English"
        }

# Syntax

1. A key is an **identifier associated with a value inside a JSON object**. 
2. All the *keys* must be enclosed in double quotes (" "). 
3. JSON is case sensitive, so *KEY* and *key* are two different keys. 
4. In JSON we can also use objects inside other objects. for eg:
    {
        "students": {
            "name" : "XYZ"
        }
    }
5. In the example above, the outermost curly braces {} define the root object. It contains all the key-value pairs and nested objects within it. Not every JSON document or JSON text needs a root object, root element can be objects, arrays, number, boolean, string, or even null.
eg: [
    "Python",
    "Java",
    "JavaScript"
]
*The above example showcases a root array*.
6. Now inside the root object, I have used the key *students* it stores another *object* which in the example has the key *name*. 
7. Basically, we can store a object inside of an object, this is called a *nested object*.
8. JSON has 6 data types, which are:
a. String =  "key" : "string"
b. Number = "key" : 123445
c. Boolean = "key" : true
d. Null =    "key" : null
e. Arrays =  "key" : [ ]
f. Objects = "key": {
                        "name": "John"
                    }
9. Now, the data you want to store must follow its respective format. For example, 
    Strings are always written in double quotes.
    Integers and floating-point numbers are written without double quotes. Both are simply treated as numbers in JSON, so there's no need to worry about separating them
    Boolean values are always *true and false*. They can't be *True and False* all the letters must be lowercase.
10. The *None* of Python is stored as *null*.
11. At the end of each data entry, if there is more to be added in the object, it should have a comma (,) separating the 2 keys.


**Every data type is present in the example file uploaded along with this Markdown file. The json file is called json.json.**
