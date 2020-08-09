# FoxQueue
`FoxQueue` is a queue implemented over array, using wrapping.

# Table of Contents

- [Installation](#installation)
- [Simple Test](#simple-test)
- [License](#license)


## Installation

```
Just copy the FoxQueue prg anywhere into your project PATH folder.
```

## Simple Test
```xBase
// declare the FoxQueue Prg
Set Procedure to "FoxQueue" Additive

// Instantiate FoxQueue Object
loQueue = CreateObject("FoxQueue")

// Enqueue some data
loQueue.Enqueue("John")
loQueue.Enqueue("Doe")
loQueue.Enqueue(1985)
loQueue.Enqueue(.T.)

// Dequeue
?"First element is: ", loQueue.Dequeue()
```

## Useful Methods
```xBase

// Enqueue() 
// Enqueue an item up the Queue. Returns the same element
?"Enqueued element:", loQueue.Enqueue("John")

// Dequeue() 
// Show the last enqueued element by modifying the Queue
?"First enqueued element is:", loQueue.Dequeue()

// Extract() 
// Extract the top element from the Queue. Returns the same element
?"Extracted element: ", loQueue.Extract()


// Clear
// Clear the Queue
loQueue.Clear()

// Count
// Returns the number of elements inside the queue.
loQueue.Count()

// Peek() 
// Show the last enqueued element without modifying the Queue
?"First enqueued element is:", loQueue.Peek()

```
## License

`FoxQueue` is released under the MIT Licence.
