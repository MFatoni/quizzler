## Objective

* Learn how to modular code into separate classes.
* Learn dart classes and objects.
* Learn how to use class constructors.
* Learn how to extract Widgets to refactor code.
* Learn about private and public modifiers in Dart.
* Learn how to use Dart lists.
* Learn the difference between var, const and final.

## Note

void main(){
  SelfDrivingCar myWaymo = SelfDrivingCar('1 Hacker Way');
}

class Car{
  int numberOfSeat = 5;
  void drive(){
    print('wheel turn');
  }
}

class SelfDrivingCar extends Car{
  String destination;
  SelfDrivingCar(String userSetDestination){
    destination=userSetDestination;
  }

  @override
  void drive(){
    void drive(){
      super.drive();
    }
    print('steering toward $destination');
  }
}

void main(){
    Human jenny = Human(height:15);
    print(jenny.height);
}

class Human{
    double height;
    Human({double height}){
        this.height= height;
    }
}

class Human{
    double height;
    Human({this.height})
}