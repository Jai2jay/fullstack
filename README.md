# hair py inheritance,polymorphism


class hair:
    def __init__(self,length,person):
        self.length = length
        self.person = person
    def type(self):
        print(f"length is{self.length}, name is{self.person}")

class curly(hair):
    def __init__(self, length, person,height):
        super().__init__(length, person) 
        self.height = height
    def type(self):
        print(f"length is:{self.length}, name is:{self.person}, height is:{self.height}")   


class straight(hair):
    def __init__(self, length, person,height):
        super().__init__(length, person) 
        self.height = height
    def type(self):
        print(f"length is:{self.length}, name is:{self.person}, height is:{self.height}")           

h1= curly("40cm","athira",167)
h1.type()
