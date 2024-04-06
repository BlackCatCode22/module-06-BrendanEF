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

---

## Lifecycle Video Code

`# class PartyAnimal:`

`#     def __init__(self):`
`#         self.x = 0`
`#         print("constructed")`

`#     def party(self):`
`#         self.x = self.x + 1`
`#         print("So far", self.x)`

`#     def __del__(self):`
`#         print("I am destructed", self.x)`


`# an = PartyAnimal()`
`# an.party()`
`# an.party()`
`# an = 42`
`# print("an contains" ,an)`

`class PartyAnimal:`

   `def __init__(self, z):`
        `self.x = 0`
        `self.name = z`
        `print(self.name, "constructed")`

    `def party(self):`
        `self.x = self.x + 1`
        `print(self.name, "party count", self.x)`

`s = PartyAnimal("Sally")`
`s.party()`
`j = PartyAnimal("Jim")`

`j.party()`
`s.party()`

### Windows PowerShell Terminal

`(.venv) PS C:\Users\Brendan\PycharmProjects\CIT95SPRING2024\CIT95python> py lifecycle_Module6.py`
`Sally constructed`
`Sally party count 1`                                                
`Jim constructed`                                                         
`Jim party count 1`                                                        
`Sally party count 2`          

---

## Inheritance Video Code

`class PartyAnimal:`

    `def __init__(self, nam):`
        `self.x = 0`
        `self.name = nam`
       `print(self.name, "constructed")`

    `def party(self):`
        `self.x = self.x + 1`
        `print(self.name, "party count", self.x)`


`class FootballFan(PartyAnimal):`

    `def __init__(self, nam):`
        `super().__init__(nam)`
        `self.points = 0`

    `def touchdown(self):`
        `self.points = self.points + 7`
        `self.party()`
        `print(self.name, "points", self.points)`


`s = PartyAnimal("Sally")`
`s.party()`

`j = FootballFan("Jim")`
`j.party()`
`j.touchdown()`

### Windows PowerShell Terminal

`(.venv) PS C:\Users\Brendan\PycharmProjects\CIT95SPRING2024\CIT95python> py inheritance_Module6.py`
`Sally constructed`
`Sally party count 1`                                                 
`Jim constructed`                                                          
`Jim party count 1`                                                        
`Jim party count 2`                                                        
`Jim points 7`          
