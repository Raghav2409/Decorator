# Decorator
The following code decorates the string with another string.

def string():
    print("Hello world")
    
def decorate(func):
    def dec():
        print("Say", end=" ")
        func()
    return dec
    
dec_string = decorate(string)
dec_string()
