XML (eXtensible Markup Language) is a versatile markup language used for structuring and encoding data in a human-readable format.

It's commonly used for document storage, configuration settings, data exchange between systems, and representing hierarchical data.

Example - 

```xml
<person>
  <name>John</name>
  <age>30</age>
</person>

```

### Tags

 XML documents consist of elements enclosed in angle brackets (<>). Elements can be nested and form a hierarchical structure.

The opening tag denotes the start of an element and contains the element name. The closing tag denotes the end of an element and contains a forward slash before the element name.

```xml
<element>content</element>
```



### Attributes 

Elements can have attributes specified within the opening tag.
    
```xml  
<user id="123" username="johndoe">
  <name>John Doe</name>
</user>
```


### Text Content

Elements can contain text content.

```xml
<description>This is an XML document.</description>

```


### comments

XML supports comments enclosed in "<! -- comment -- >" tags.

```xml
<!-- This is a comment -->
```



### Whitespace

While whitespace is often insignificant, it can be preserved for readability using CDATA or specific XML formatting settings..



### Document Declaration

XML documents typically start with a declaration specifying the version and encoding.

```xml
<?xml version="1.0" encoding="UTF-8"?>

<person>
  <name>John</name>
  <age>30</age>
</person>
```

XML documents must adhere to strict syntax rules to be well-formed, including properly nested elements and closing tags.

In summary, XML is a versatile markup language for representing structured data. It uses elements, attributes, and various features to encode data for diverse use cases, including data interchange, configuration, and document storage. Proper adherence to XML rules is essential for creating well-formed documents.

<br>

### Examples

#### Book Catalog 

```xml
<?xml version="1.0" encoding="UTF-8"?>
<catalog>
  <book>
    <title>Harry Potter and the Sorcerer's Stone</title>
    <author>J.K. Rowling</author>
    <price>29.99</price>
  </book>
  <book>
    <title>The Catcher in the Rye</title>
    <author>J.D. Salinger</author>
    <price>19.99</price>
  </book>
</catalog>

```

<br>

#### Student Records 

```xml
<?xml version="1.0" encoding="UTF-8"?>
<students>
  <student>
    <name>John Doe</name>
    <id>12345</id>
    <courses>
      <course>Mathematics</course>
      <course>Physics</course>
      <course>History</course>
    </courses>
  </student>
  <student>
    <name>Alice Smith</name>
    <id>67890</id>
    <courses>
      <course>English</course>
      <course>Chemistry</course>
      <course>Art</course>
    </courses>
  </student>
  <!-- Add more student records as needed -->
</students>
```

<br>
<br>
<br>
<br>
