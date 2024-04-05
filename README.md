[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/OLjHVbQB)
# tPythonModule06

Code up the three short programs in this module:

sampleClass, lifecycle, inheritance

## Sample Class Video Code

`class PartyAnimal:`
    `def __init__(self):`
        `self.x = 0`

    `def party(self):`
        `self.x = self.x + 1`
        `print("So far",self.x)`

`an = PartyAnimal()`

`an.party()`
`an.party()`
`an.party()`

`print("Type", type(an))`
`print("Dir ", dir(an))`
`print ("Type", type(an.x))`
`print ("Type", type(an.party))`

### Windows PowerShell Terminal

`(.venv) PS C:\Users\Brendan\PycharmProjects\CIT95SPRING2024\CIT95python> py sampleClass_Module6.py`
`So far 1`
`So far 2`
`So far 3`
`Type <class '__main__.PartyAnimal'>`
`Dir  ['__class__', '__delattr__', '__dict__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getstate__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__le__', '__lt__', '__module__', '
__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', '__weakref__', 'party', 'x']`
`Type <class 'int'>`
`Type <class 'method'>`
