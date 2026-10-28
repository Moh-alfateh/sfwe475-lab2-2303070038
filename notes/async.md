# Async notes

# Strand 1: while await fetch is waiting, what can the rest of the program do?

Only the function that contains the await stops and waits. The rest of the program keeps running, because JavaScript does not freeze while the answer travels over the network. When the response arrives, the paused function continues from the same line. It is like placing an order in a restaurant: you do not stand at the kitchen door, you can do other things until the food is ready.