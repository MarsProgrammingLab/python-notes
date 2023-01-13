# Escaping
- To include any quotes in your string, use the backslash symbol (`\`) before the quotes inside of the string. The backslash will basically tell Python that the quote symbol that follows it is a part of the string rather than its end or beginning. It is called escaping.

## Examples 

    print("You're doing great!")
    print('You\'re doing great!')
    print("Have you read \"Hamlet\"?")
    print('Have you read "Hamlet"?')

## Raw Strings
- "r" at the beginning of a string will treat the string as a "raw string", allowing output of characters without escaping.   