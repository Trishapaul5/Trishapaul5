#stack operation using list in python 
class Stack:
    """
    Implementation of a stack in Python using lists.
    """

    def __init__(self):
        """
        Initializes an empty stack.
        """
        self.stack_data = []  # Empty list to store the data for the stack.

    def push(self, value):
        """
        Pushes/adds a value to the end of the stack.
        :param value: object - A value of any data type that needs to be stored in the stack.
        """
        self.stack_data.append(value)

    def pop(self):
        """
        Pops/removes the last value from the stack.
        Prints a message if the stack is empty.
        """
        if len(self.stack_data) == 0:
            print("Stack is empty. Nothing to pop.")
        else:
            return self.stack_data.pop()

    def display_stack(self):
        """
        Displays the elements present in the stack by printing each element.
        If the stack is empty, prints a message.
        """
        if len(self.stack_data) == 0:
            print("Stack is empty.")
        else:
            print("Stack contents:", self.stack_data)


def main():
    """
    The main function of the program.
    """
    stack_obj = Stack()  # Creating the stack object.
    stack_obj.display_stack()  # Display the contents of the stack (initially empty).

    # Adding values to the stack:
    stack_obj.push(10)
    stack_obj.push(1)
    stack_obj.push(34)
    stack_obj.push(56)
    
    stack_obj.display_stack()  # Display the contents of the stack after adding elements.

    # Popping a value from the stack:
    popped_value = stack_obj.pop()
    print(f"Popped value: {popped_value}")

    # Display stack after popping:
    stack_obj.display_stack()

if __name__ == "__main__":
    main()
# QUEUE OPERATION USING LISTS 
class Queue:
    """
    Implementation of a queue in Python using lists.
    """

    def __init__(self):
        """
        Initializes an empty queue.
        """
        self.queue_data = []  # Empty list to store the data for the queue.

    def push(self, value):
        """
        Pushes/adds a value to the end of the queue.
        :param value: object - A value of any data type that needs to be stored in the queue.
        """
        self.queue_data.append(value)

    def pop(self):
        """
        Pops/removes the first value from the queue (FIFO).
        Prints a message if the queue is empty.
        """
        if len(self.queue_data) == 0:
            print("Queue is empty. Nothing to pop.")
        else:
            return self.queue_data.pop(0)

    def display_queue(self):
        """
        Displays the elements present in the queue by printing each element.
        If the queue is empty, prints a message.
        """
        if len(self.queue_data) == 0:
            print("Queue is empty.")
        else:
            print("Queue contents:", self.queue_data)


def main():
    """
    The main function of the program.
    """
    queue_obj = Queue()  # Creating the queue object.
    queue_obj.display_queue()  # Display the contents of the queue (initially empty).

    # Adding values to the queue:
    queue_obj.push(10)
    queue_obj.push(1)
    queue_obj.push(34)
    queue_obj.push(56)

    queue_obj.display_queue()  # Display the contents of the queue after adding elements.

    # Popping values from the queue:
    popped_value = queue_obj.pop()
    print(f"Popped value: {popped_value}")
    
    queue_obj.display_queue()  # Display the contents after popping.

    popped_value = queue_obj.pop()
    print(f"Popped value: {popped_value}")

    queue_obj.display_queue()  # Display the contents after popping another element.


if __name__ == "__main__":
    main()
