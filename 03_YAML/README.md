YAML (YAML Ain't Markup Language) is a human-readable data serialization format used for configuration files, data exchange, and representing hierarchical data structures.

It's commonly used in software configuration files, Kubernetes manifests, and as a data interchange format.

Example - 

```yaml
person:
  name: Yash
  age: 20

```

### Key-Value Pairs

YAML data is typically represented as key-value pairs using colons : to separate keys and values.

```yaml
name: Yash
age: 20
```


### Indentation

YAML uses indentation (whitespace) to indicate nesting. It's crucial for defining the structure of the data.

```yaml
person:
  name: Bob
  age: 35
```


### Lists 

YAML supports lists or arrays of values, which are represented using hyphens - followed by a space.

```yaml
fruits:
  - apple
  - banana
  - cherry
```



### Scalars

Scalars in YAML can be plain values (e.g., strings, numbers, booleans) without any special characters.

```yaml
message: Hello, world!
score: 95.5
isStudent: true
```


### Multiline Strings 

You can represent multiline strings using the | or > symbol. | preserves newlines, while > folds them into spaces.

```yaml
description: |
  This is a multiline
  YAML string.
```



### Comments

YAML supports comments using the # symbol. Comments are for documentation and not part of the data.

```yaml
# This is a comment
name: Yash
```



### Objects and Nested Structures

YAML can represent nested objects and structures.

```yaml
person:
  name: Carol
  address:
    street: 123 Main St
    city: Anytown
```


### Null Value

YAML can represent a null value using null.

```yaml
data: null
```



### Anchors and Aliases

YAML allows you to define anchors (&) and aliases (*) to reuse data across the document.

#### Anchors 

- An anchor is a unique identifier (usually a name) that you assign to a YAML data structure (e.g., a map, list, or scalar value) using the & symbol followed by the anchor name.

- Anchors are used to mark a point in the YAML document where you want to "store" a piece of data for later reference.

- Anchors are typically placed immediately before the data structure you want to anchor.


```yaml     
# Define an anchor for a map (object)
user_data: &user_anchor
  name: John
  age: 30

# Define an anchor for a list (array)
fruits: &fruits_anchor
  - apple
  - banana
  - cherry

```


#### Aliases

- An alias is a reference to an anchor within the YAML document, allowing you to reuse the anchored data at another location in the document.

- Aliases are created using the * symbol followed by the anchor name you want to reference.

- Aliases are typically used where you want to include the anchored data, effectively "copying" it from the anchor point.


```yaml
# Reference the user_data anchor using an alias
user_copy: *user_anchor

# Reference the fruits anchor using an alias within a list
grocery_list:
  - milk
  - bread
  - *fruits_anchor
  - eggs

```


```yaml
user_data: &user_anchor
  name: John
  age: 30
fruits: &fruits_anchor
  - apple
  - banana
  - cherry



user_copy: *user_anchor
grocery_list:
  - milk
  - bread
  - *fruits_anchor
  - eggs
```


In summary, YAML is a human-readable and whitespace-sensitive data serialization format that is commonly used for configuration files and representing structured data. Its simplicity and readability make it a popular choice for various applications like Configuration Files, Application Configuration etc.



Examples of yaml - 

1. Web Application Configuration

```yaml
app_name: MyWebApp
port: 8080
debug_mode: true

database:
  host: localhost
  port: 5432
  name: mydb
```


2. Kubernetes Manifest

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
spec:
  replicas: 1
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
        - name: nginx
          image: nginx:latest
          ports:
            - containerPort: 80
```


<br>
<br>
<br>
<br>