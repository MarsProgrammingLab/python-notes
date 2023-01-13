# List

List are: 

- Ordered, i.e. each element has a fixed position in a list;
- Iterable, i.e. you can get their elements one by one;
- Able to store duplicate values;
- Able to store different types of elements;
- Besides being used for creating an empty list, the list() function also can be used to make a list out of an iterable object.

## Creating and printing a list
Example:
    
    dog_breeds = ['corgi', 'labrador', 'poodle', 'jack russell']
    print(dog_breeds)  # ['corgi', 'labrador', 'poodle', 'jack russell']

## Difference between list function and creating a list using square brackets 
    
    # List using list function
    multi_element_list = list('danger!')
    print(multi_element_list)  # ['d', 'a', 'n', 'g', 'e', 'r', '!']
    
    # List created using square brackets
    single_element_list = ['danger!']
    print(single_element_list)  # ['danger!']

## Indexes

- Positionally ordered collections of elements are usually called sequences, and both lists and strings belong to them
- Each element in a list, as well as each character in a string, has an index that corresponds to its position. 
- Indexes are used to access elements within a sequence. Indexing is zero-based.

- To access an element of a list by its index, you need to use square brackets. You add the brackets after the list and, between them, you write the index of an element you want to get.

- The index of the first element is 0. The index of the last element is equal to len(list) - 1.

Example:

    colors = ['red', 'green', 'blue']

    first_elem = colors[0]   # 'red'
    second_elem = colors[1]  # 'green'
    third_elem = colors[2]   # 'blue'

Strings example:

    pet = "cat"

    first_char = pet[0]   # 'c'
    second_char = pet[1]  # 'a'
    third_char = pet[2]   # 't'

An element can be changed in a list as follows: 

    colors = ['red', 'green', 'blue']

    colors[1] = 'white'
    print(colors)  # ['red', 'white', 'blue']

However, when it comes to strings, such reassignment is impossible. Strings, unlike lists, are immutable, so you can't modify their contents with indexes:

    pet = "cat"

    pet[0] = "b"
    # TypeError: 'str' object does not support item assignment

## Negative indexes

The easier way to access the elements at the end of a list or a string is to use negative indexes: the minus before the number changes your perspective in a way and you look at the sequence from the end. So, the last element of a list, in this case, has the index equal to -1, and the first element of the list has the index -len(list) (the length of the list).

For example:

    colors = ['red', 'green', 'blue']

    last_elem = colors[-1]    # 'blue'
    second_elem = colors[-2]  # 'green'
    first_elem = colors[-3]   # 'red'

    pet = "cat"

    last_char = pet[-1]    # 't'
    second_char = pet[-2]  # 'a'
    first_char = pet[-3]   # 'c'

As you can see, it works the same for lists and strings.

If you write a non-existing negative index, you'll also get IndexError. Be careful with indexes to avoid off-by-one errors in your code.
