# What is JSON
### JavaScript Object Notation
* Data Representation Format
* Commonly used for APIs and Configs
* Lightweight and Easy to Read/Write
* Integrates Easily with Most Languages

### JSON Data Types
* Strings - "Hello World" "Hyuk" 
* Numbers - 10 1.5 -30 1.2e10
* Booleans - true false
* Null - null
* Array - [1,2,3] ["Hello World","Good Bye"]
* Object {"key":"value"} {"age":30}

### JSON Sample
```javascript
[
    {
        "name": "Big Corporation",
        "numberOfEmployees": 10000,
        "ceo": "Mary",
        "rating": 3.6
    },
    {
        "name": "Small Startup",
        "numberOfEmployees": 3,
        "ceo": null,
        "rating": 4.3
    }
]
```

### JSON Parse Example 1
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>JSON Example</title>
</head>
<body>
    <script type="text/javascript">
        let companies = 
        [
            {
                "name": "Big Corporation",
                "numberOfEmployees": 10000,
                "ceo": "Mary",
                "rating": 3.6
            },
            {
                "name": "Small Startup",
                "numberOfEmployees": 3,
                "ceo": null,
                "rating": 4.3
            }
        ]
        console.log(companies[0].name);
    </script>
</body>
</html>
```

### JSON Parse Example 2
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>JSON Example</title>
</head>
<body>
    <script type="text/javascript">
        let companies = 
        `
        [
            {
                "name": "Big Corporation",
                "numberOfEmployees": 10000,
                "ceo": "Mary",
                "rating": 3.6
            },
            {
                "name": "Small Startup",
                "numberOfEmployees": 3,
                "ceo": null,
                "rating": 4.3
            }
        ]`
        console.log(JSON.parse(companies)[1].name);
    </script>
</body>
</html>
```