# What are you doing?
### Charles M. Schwab  

``` Swift: v4 ```

```swift
var QuoteAuthor = "Charles M. Schwab"
var grub = "sleepdeficit"

struct Person {
    var withName: String, withResponse: Int
    init(_ name: String, _ index: Int) { withName = name; withResponse = index }
}

var BrickLayers: [Person] = [Person("Alice: ", 0), Person("Bob: ", 1), Person("Eve: ", 2)]

var question = ["What are you doing? \n", "What are you working for? \n", "What are you doing? \n"]
var response = ["Laying some brick. \n", "Five dollars a day. \n", "I am helping to build a great cathedral. \n"]

func ask(_ person: Person) -> String { return question[person.withResponse] }
func answer(from person: Person) -> String {  return response[person.withResponse] }

for person in BrickLayers {
    print(ask(person), person.withName + answer(from: person))
}
```
#
