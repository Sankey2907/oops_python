# oops_python
#This python code for class inheritance
# create a clsss

class car:
    #add _ init__() method
    def __init__(self,cname,brand):
        self.cname = cname
        self.brand = brand
    def myfunc(self):
        print("Car" +self.cname+ "brand" +self.brand)
c4 = car(" SRT "," Arbath ")
c4.myfunc()
c1 = car("Accent","hyundai")
c2 = car("swift","Maruti")
print("The car name is ", c1.cname)
print("The brand name is", c1.brand)
print("The car name is ", c2.cname)
print("The brand name is", c2.brand)
c3 = car("audi","Volkswagen")
print("The car name is ", c3.cname)
print("The brand  is ",c3.brand)

#class inheritance
#1 single
#2 multiple 
#3 Multilevel 
#4 hirarical 
#5 Hybrid 

#single 


class company:
    def func_01(self):
        print("The car company name is Volkswagen ")
class car:
    def func_02(self):
        print("The car name is Audi")
class model:
    def func_03(self):
        print("the car model is A6")
ob = company()
ob.func_01()
# multiple inheritance 
class subsidarie1:
    def func1(self):
        print("The subsidarie is skoda")
class subsidarie2:
    def func2(self):
        print("The subsidare2 is Porche")
class car(subsidarie1,subsidarie2):
    def func3(self):
        print("this is the car company")
ob = car()
ob.func1()
ob.func2()
ob.func3()
#multilevel inheritance 
class company:
    def func1(self):
        print("the company is suzuki")
class car1(company):
    def func2(self):
        print("swift belong to suzuki")
class car2(company):
    def func3(self):
        print("car belong to suzuki")
ob1 = company()
ob2 = car1()
ob3 = car2()
ob.func3()
ob.func2()
ob.func1()
### hirarchical  inheritance \
class Brands:
    brand_name_1 = "Audi"
    brand_name_2 = "Thar"

class Type(Brands):
    type_1 = "Luxury"
    type_2 = "offroader"

class popularity(Brands):
    pop_1 = 98
    pop_2 = 80

class value(Brands):
    val_1 = "EXcellent"
    val_2 = "Medium"

obj_1 = Type()
obj_2 = popularity()
obj_3 = value()
print(obj_1.brand_name_1+" is a "+obj_1.type_1)
print(obj_1.brand_name_2+" is an "+obj_1.type_2)



### Hybrid inheritance 
class Vehicle:
    def __init__(own):
        print("Vehicle")
class  Bike(Vehicle):
    def __init__(own):
        super().__init__()
        print("Bike")
class  Car(Vehicle):
    def  __init__(own):
        super().__init__()
        print("Car")
class  movables(Bike,Car):
    def __init__(own):
        super().__init__()
        print("movables")
c = movables()
 #sanka
