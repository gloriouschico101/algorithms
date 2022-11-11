## Lists

A list data structure is a collection data type that allows multiple values to be stored within the same field. Lists are stored in certain chunks of memory which are linked together with pointers, that allows
efficient use of memory and doesn't require resizing.


`"apple"`, `"orange"`, `"carrot"` and `"pear"` are being stored in a list named `foods` and the list gets printed out.
It then adds `"chocolate"` and `"cake"` to the list, which automatically changes the size of the list. Then prints the list out

    foods = ["apple", "orange", "carrot", "pear"]
    
    for i in foods:
        print(i)

    print("")
    print("")

    foods.append("chocolate")
    foods.append("cake")
    
    for i in foods:
        print(i)


## Arrays

An array data structure is a data structure that is a fixed size, can be dynamically reallocated, and is efficiently indexed.
It stores multiple items of the same type together, which makes it easier to calculate the position of each element.
It can not store different types such as integers and floats in one array.


We first have to import array as it is before we can use arrays.
`1`, `2`, `3` and `4` are integer numbers and are being stored into an integer array named `int_array` and then gets printed out.
`1.1`, `2.2`, `3.3` and `4.4` are float numbers, that are being stored into a float array named `float_array` and then gets printed out.
The `'i'` in the `int_array` indicates that it is an integer array and only integer numbers can be put into the array.
The `'f'` in the `float_array` indicates that it is a float array and only float numbers can be put into the array

    import array

    int_array = array.array('i', [1, 2, 3, 4])
    float_array = array.array('f', [1.1, 2.2, 3.3, 4.4])

    for i in int_array:
        print(i)

    for a in float_array:
        print(a)



## Linked Lists

Linked lists are an ordered collection of objects. Linked lists are different from lists because of the way they store elements in memory.
While lists use a contiguous memory block to store references to their data, linked lists store references as a part of their own element.


## Stack

A stack is a linear data structure that stores items in a LIFO (Last-In/First-Out) way. So the last element you add to the stack, will be the first element to come off the stack.
The insert and delete operations are usually called push and pop.

We have 3 elements being added to the stack: `1`, `2` and `3`. Because `3` was added on last, the first pop will remove `3` from the stack, then remove `2`, and then finally `1`.

    stack = []

    stack.append(1)
    stack.append(2)
    stack.append(3)

    print("First stack")
    print(stack)

    print("Popped from stack:")
    print(stack.pop())
    print(stack.pop())
    print(stack.pop())

    print("Stack after the pops")
    print(stack)

## Queues

Queues are like stacks in the fact that they are a linear data structure. However, they store items in FIFO (First-In/First-Out) way. So the first element to be added to the stack, will be the first
element to come off the stack.


We have 3 elements being added to the queue: `1`, `2` and `3`. Because `1` was added on first, the first pop will remove `1` from the stack, then remove `2`, and then finally `3`.

    queue = []

    queue.append(1)
    queue.append(2)
    queue.append(3)

    print("First queue")
    print(queue)

    print("Dequeued from queue")
    print(queue.pop(0))
    print(queue.pop(0))
    print(queue.pop(0))

    print("Queue after the dequeing")
    print(queue)

## Trees



## Graphs

Graphs are complex, non-linear data structures that are made by a group of vertices, connected by edges.

`Vertices` - Vertices are what's in a graph. Every vertex has a value that is associated with it. An example would be a list of houses using a graph, the vertices would represent the houses.
`Edges` - Edges is the relationship between the vertices in the graph. Edges may or may not have a vlue associated with them. An example would be a list of towns using a graph, the edges would be the
road between the houses.

Here we have a graph that has 3 vertices. The cost of moving from vertex 0 to vertex 1 is 1. Where as the cost of moving from vertex 0 to vertex 2 is 2.
When moving from a vertex to itself, it is usually 0.

    graph = [[0, 1, 2],
             [2, 0, 5],
             [4, 5, 0]]

## Sets

A set data structure is an unordered collection of items. Every element is unique meaning there cannot be duplicates of an element, and cannot be changed.
However, you can add or remove items from it.
A set is created by placing all the elements inside curly braces `{}`, seperated by comma.

Here, we have a set of values `1`, `2`, `3`, `4`, `3` and `2`. However, after the `4`, the `3` and `2` are not added as they are duplicates.
So we get an output of `{1, 2, 3, 4}`

    my_set = {1, 2, 3, 4, 3, 2}
    print(my_set)


## Hash tables

Hash tables are a type of data structure that the index value of the data element is generated from a hash function. This makes accessing data faster as the index value is like a key for the data value.
In Python, the Dictionary data types represent the implementation of hash tables.

Here, we have 3 keys:
`Name` - With the data value: `Callum`
`Age` - With the data value: `20`
`Class` - With the data value: `Programming`

We can then print out the `Name` and `Age` by using the key.

    dict = {'Name': 'Callum', 'Age': '20', 'Class': 'Programming'}

    print("Name: ", dict['Name'])
    print("Age: ", dict['Age'])