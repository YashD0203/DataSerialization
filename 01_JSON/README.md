# JSON 

JSON (JavaScript Object Notation) is a lightweight data-interchange format that is easy for both humans and machines to read and write. It is often used to transmit data between a server and a web application, store configuration settings, and more.

JSON data is represented as key-value pairs, where keys are strings and values can be various data types like strings, numbers, objects, arrays, booleans, or null.



### Object
JSON data is often structured as a collection of key-value pairs enclosed in curly braces {}. Each key is a string enclosed in double quotes, followed by a colon :, and then a value. Keys must be unique within an object.

```json
{
  "name": "Yash",
  "age": 20,
  "city": "New Delhi"
}
```



### Array   
JSON data can also be structured as an array. An array is a comma-separated list of values enclosed in brackets []. Just like objects, arrays can contain any combination of data types.

```json
{
  "name": "Yash",
  "age": 20,
  "cities": ["New Delhi", "Mumbai", "Bangalore"]
}
```



### Nested Objects and Arrays
JSON data can be nested. The value of a key can also be another object or an array.

```json
{
  "name": "Yash",
  "age": 20,
  "cities": ["New Delhi", "Mumbai", "Bangalore"],
  "friends": [
    {
      "name": "Rahul",
      "age": 20
    },
    {
      "name": "Rohit",
      "age": 20
    }
  ]
}
```



### Strings 
Strings in JSON must be enclosed in double quotes.

```json
{
  "message": "Hello, world!"
}
```



### Numbers 
JSON supports numbers, which can be integers or floating-point numbers.

```json
{
  "age": 20,
  "pi": 3.14
}
```



### Booleans
JSON supports boolean values true and false.

```json
{
  "isMarried": false
}
```



### Null
JSON supports null, which represents the absence of a value.

```json
{
  "car": null
}
```



### Whitespace
JSON ignores whitespace. You can add whitespace to make it more readable.



### Encoding and Escaping 
When writing JSON in a programming language, you usually don't need to worry about manual escaping, as most programming languages handle it for you when converting data structures to JSON. However, if you're manually creating JSON, you should escape special characters within strings, such as double quotes ("), backslashes (\), and control characters.

escaping is used to include special characters without causing syntax errors. For instance, escaping double quotes (") in a JSON string.


```json
{
  "message": "This is a \"quoted\" string."
}
```

In the above example, \" is used to escape the double quotes within the JSON string. This indicates that the double quotes are part of the string's content


<br>

JSON is primarily used for data interchange and is not a full-fledged programming language. When working with JSON in code, you typically parse it into data structures provided by your programming language and then manipulate those structures. Similarly, you can convert data structures back into JSON when you need to send data. JSON libraries are available in most programming languages to help with this process.
