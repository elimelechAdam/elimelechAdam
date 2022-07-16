// // 'use strict';

// const Person = function (firstName, birthYear) {
//   this.firstName = firstName;
//   this.birthYear = birthYear;

//   //   console.log(firstName, this.firstName);
//   //   console.log(birthYear, this.birthYear);

//   // Never do this
//   //   this.calcAge = function () {
//   //     console.log(2037 - this.birthYear);
//   //   };
// };

// const adamas = new Person('Adam', 1995);

// Person.Hey = function () {
//   console.log('Hey :)))) Person.Hey');
// };
// Person.Hey();

// // // // 1. New {} is created
// // // // 2. function is called, this = {}
// // // // 3. {} linked to prototype
// // // // 4. function automatically return {}

// // // const adame = new Person('Elime', 2004);

// // // // Prototypes
// // // Person.prototype.calcAge = function () {
// // //   console.log(2022 - this.birthYear);
// // // };
// // // adam.calcAge();
// // // adame.calcAge();
// // // Person.prototype.species = 'human';

// // // console.log(adam);

// // // console.log(adam.__proto__);
// // // // Object.prototype
// // // console.log(adam.__proto__.__proto__);
// // // // null
// // // console.log(adam.__proto__.__proto__.__proto__);

// // // console.dir(Person.prototype.constructor);

// // // const arr = [1, 3, 4, 4, 1, 34, 3]; // new Array === []
// // // console.log(arr.__proto__);
// // // console.log(arr.__proto__.__proto__);

// // // Array.prototype.unique = function () {
// // //   return [...new Set(this)];
// // // };

// // // console.log(arr.unique());

// // ///////////////////////////////////
// // ///////////////////////////////////
// // //////////// Study ////////////////
// // ///////////////////////////////////
// // ///////////////////////////////////
// // /*

// // 1. User a constructor function to implement a Car.
// // A car has make and a speed property. The speed
// // property is the currect speed of the car in km/h;
// // 2. Implement an 'accelerate' method that will
// // increase the car's speed by 10, and log the new speed
// // to the console;
// // 3. Implement a 'break' method that will decrease the
// // car's speed by 5, and log the new speed to the console;
// // 4. Create 2 car objects and experminet with calling
// // 'accelerate' and 'brake' multiple times on each of
// // them.

// // DATA CAR 1: 'BMW' going at 120 km/h
// // DATA CAR 2: 'Mercedes' going at 95 km/h

// // */

// // const Cars = function (make, speed) {
// //   this.make = make; //currect speed
// //   this.speed = speed; //currect speed
// //   // console.log(this);
// //   // console.log(speed);
// //   // console.log(this.speed);
// // };

// // Cars.prototype.accelerateCar = function () {
// //   // this.speed
// //   this.speed += 10;
// //   console.log(`${this.make} currectly speeding at ${this.speed} km/h`);
// // };
// // Cars.prototype.breakCar = function () {
// //   // this.speed
// //   this.speed -= 5;
// //   console.log(
// //     `${this.make} currectly at breaking, Speed at: ${this.speed} km/h`
// //   );
// // };

// // const bmwCar = new Cars('BMW', 120);
// // const MercedesCar = new Cars('Mercedes', 95);
// // const Audi = new Cars('Audi', 100);
// // const AudiR8 = new Cars('AudiR8', 150);

// // bmwCar.accelerateCar();
// // bmwCar.accelerateCar();
// // bmwCar.breakCar();
// // bmwCar.breakCar();
// // bmwCar.accelerateCar();

// // Audi.accelerateCar();
// // Audi.accelerateCar();
// // Audi.accelerateCar();
// // Audi.accelerateCar();

// // AudiR8.accelerateCar();
// // AudiR8.accelerateCar();
// // AudiR8.accelerateCar();

// // class expression
// // const PersonA = class {};

// //ES6
// // class declaration
class Person {
  constructor(fullName, birthYear) {
    this.fullName = fullName;
    this.birthYear = birthYear;
  }
  //Instance methods
  sayHello() {
    console.log(`Hello ${this.fullName}`);
  }
  adminHello() {
    console.log(`This MSG brought to you by ADMIN`);
  }
  get getAge() {
    return 2037 - this.birthYear;
  }

  // Set a property that already exists
  set fullName(fullName) {
    console.log(fullName);
    if (fullName.includes(' ')) this._fullName = fullName;
    else console.log(fullName, ' doesnt exist');
  }
  get fullName() {
    return this._fullName;
  }

  //Static method
  static hey() {
    console.log('Hey :)))) static.Hey');
  }
}

// console.log(adam.getAge);
// PersonA.hey();

// // adam.sayHello();
// // sss.sayHello();

// // 1. Classes are NOT hoisted
// // 2. Classes are first-class citizes
// // 3. Classes are executed in strict mode

// const walter = new PersonA('Walter', 1965);

// const account = {
//   owner: 'Adam',
//   movements: [200, 100, 150, 88],
//   get lastestMovements() {
//     // without the POP function it would stay in array
//     return this.movements.slice(-1).pop();
//   },

//   set lastestMovements(mov) {
//     // console.log(this); // Contains all the data
//     // console.log(mov); // Contains only the movement itself
//     // console.log(this.movements); // contain the array of movements
//     this.movements.push(mov);
//   },
// };
// // console.log(account.lastestMovements);
// // account.lastestMovements = 20; //add to - set lastestMovements(mov)
// // console.log(account);

// const PersonProto = {
//   calcAge() {
//     return 2037 - this.birthYear;
//   },

//   init(firstName, birthYear) {
//     this.firstName = firstName;
//     this.birthYear = birthYear;
//   },
// };
// const steven = Object.create(PersonProto);
// // console.log(steven);
// steven.fullName = 'Steven Barkins';
// steven.birthYear = 1999;

// // console.log(steven.calcAge());
// // console.log(steven);

// const sarah = Object.create(PersonProto);
// // console.log(sarah);
// // sarah.init('Sarah', 1540);
// // console.log(sarah);
// // console.log(sarah.calcAge());

// /////////////////////////////////
// // Coding challenge #2

// /*
// 1. Recreate challenge 1. but this time using an ES6 class;
// 2. Add a getter called 'SpeedUS' which returns the currect
// speed in mi/h(divide by 1.6);
// 3. Add a seeter called 'SpeedUS' which sets the curerct speed
// in mi/h (but converts it to km/h before storing the value,by multiplaying
// the input by 1.6);
// 4. Create a new car and experiment with the accelerate and brake methods,
// and with the getter and setter;

// DATA CAR 1: 'Ford' going at 120 km/h

// */
// // const Cars = function (make, speed) {
// //   this.make = make; //currect speed
// //   this.speed = speed; //currect speed
// //   // console.log(this);
// //   // console.log(speed);
// //   // console.log(this.speed);
// // };

// // Cars.prototype.accelerateCar = function () {
// //   // this.speed
// //   this.speed += 10;
// //   console.log(`${this.make} currectly speeding at ${this.speed} km/h`);
// // };
// // Cars.prototype.breakCar = function () {
// //   // this.speed
// //   this.speed -= 5;
// //   console.log(
// //     `${this.make} currectly at breaking, Speed at: ${this.speed} km/h`
// //   );
// // };

// class Car {
//   constructor(make, speed) {
//     this.make = make;
//     this.speed = speed;
//   }
//   accelerate() {
//     this.speed += 10;
//     console.log(`${this.make} has acclerate ,currect speed: ${this.speed}`);
//   }
//   break() {
//     this.speed -= 5;
//     console.log(`${this.make} has breaked ,currect speed: ${this.speed}`);
//   }
//   get SpeedUS() {
//     //Add a getter called 'SpeedUS' which returns the currect speed in mi/h(divide by 1.6);
//     const speedInMiles = this.speed / 1.6;
//     console.log(`Speed in MI/H: ${speedInMiles}`);
//   }
//   set SpeedUS(speed) {
//     /*Add a seeter called 'SpeedUS' which sets the curerct speed
//       in mi/h (but converts it to km/h before storing the value,by multiplaying
//       the input by 1.6);
//    */
//     this.speed = speed * 1.6;
//     console.log(`Speed in KM/H: ${this.speed}`);
//   }
// }

// const ford = new Car('Ford', 120);
// console.log(ford.speed);

// ford.accelerate();
// ford.accelerate();
// ford.break();
// ford.SpeedUS;
// ford.SpeedUS = 50;

////////////////////////////
// Inheritance between "Classes" : Constructor Functions
// const Person = function (firstName, birthYear) {
//   this.firstName = firstName;
//   this.birthYear = birthYear;
// };

// Person.prototype.calcAge = function () {
//   console.log(2037 - this.birthYear);
// };

// const Student = function (firstName, birthYear, course) {
//   Person.call(this, firstName, birthYear);
//   this.course = course;
// };
// Student.prototype = Object.create(Person.prototype);
// Student.prototype.constructor = Student;

// Student.prototype.intro = function () {
//   console.log(
//     `Hi my name is ${this.firstName} and my course is : ${this.course}`
//   );
// };

// const mike = new Student('Mike', 1995, 'Computer Science');
// const mikess = new Student('Mikesss', 1995, 'Computer Scsience');

// mike.intro();
// mike.calcAge();
// mikess.intro();
// console.log(mike);
// console.dir(Student.prototype.constructor);

/*
  1. Use a constructor function to implement an electric car(EV)
  as a CHILD "class" of Car.
  Besides a make a cuurect speed, the EV also has currect battery
  charge in %('charge' property);
  2. Implement a 'chargeBattery' method which takes an argument
  'chargeTo' and sets the battery charge to 'chargeTo'
  3. Implement an 'accelerate' method that will increase the cars
  speed by 20 and decrese the charge by 1%. then log a message like this:
  'Tesla going at 140 km/h ,with a charge of 22%';
  4. Create an electric car object and experiment with calling
  'accelerate' ,'brake' and 'chargeBattery'(charge to 90%); notice
  what happens when you 'accelerate'!
  HINT: Review the fedinion of polymorphism

  DATA CAR 1: Tesla going at 120 km/h ,with a charge of 23%

*/

// const Car = function (make, speed) {
//   this.make = make;
//   this.speed = speed;
// };

// Car.prototype.acclerate = function () {
//   this.speed += 10;
//   console.log(`${this.make} has acclerate ,currect speed: ${this.speed}`);
// };
// Car.prototype.brake = function () {
//   this.speed -= 5;
//   console.log(`${this.make} has braked ,currect speed: ${this.speed}`);
// };

// const EV = function (make, speed, battery) {
//   Car.call(this, make, speed);
//   this.battery = battery;
// };
// EV.prototype = Object.create(Car.prototype);

// //2. Implement a 'chargeBattery' method which takes an argument 'chargeTo' and sets the battery charge to 'chargeTo'
// EV.prototype.chargeBattery = function (chargeTo) {
//   this.chargeTo = chargeTo;
// };

// //3.Implement an 'accelerate' method that will increase the cars speed by 20 and decrese the charge by 1%. then log a message like this:
// //'Tesla going at 140 km/h ,with a charge of 22%';
// EV.prototype.accelerate = function (make, speed, battery) {
//   this.speed += 20;
//   this.battery--;
//   console.log(
//     `${this.make} going at ${this.speed} km/h, with a charge of ${this.battery}%`
//   );
// };
// //4. Create an electric car object and experiment with calling 'accelerate' ,'brake' and 'chargeBattery'(charge to 90%); notice
// // what happens when you 'accelerate'!

// const Tesla = new EV('Tesla', 120, 23);
// console.log(Car);
// console.log(Tesla);
// Tesla.accelerate();
// Tesla.accelerate();

// Tesla.brake();

// class Student extends Person {
//   constructor(fullName, birthYear, course) {
//     // Always needs to happen first
//     super(fullName, birthYear);
//     this.course = course;
//   }
//   welcomeMsg() {
//     console.log(`Welcome ${this.fullName}`);
//   }
// }
// const Adam = new Student('Adam Elimelech', 1995, 'CS');
// Adam.welcomeMsg();
// console.log(Adam.getAge);
// Adam.adminHello();

// const PersonProto = {
//   calcAge() {
//     return 2037 - this.birthYear;
//   },

//   init(firstName, birthYear) {
//     this.firstName = firstName;
//     this.birthYear = birthYear;
//   },
// };
// const steven = Object.create(PersonProto);

// const StudentProto = Object.create(PersonProto);
// StudentProto.init = function (firstName, birthYear, course) {
//   PersonProto.init.call(this, firstName, birthYear);
//   this.course = course;
// };
// const jacky = Object.create(StudentProto);

// const alex = Object.create(StudentProto);

// jacky.init('Jacky', 1999, 'CS');
// steven.init('Steven', 1995);
// alex.init('Alex', 2000, 'PHP');
// console.log(steven.calcAge());
// console.log(alex);
// console.log(jacky);
// console.log(steven);
// class Account {
//   constructor(owner, currency, pin) {
//     this.owner = owner;
//     this.currency = currency;
//     // Protected property
//     this._pin = pin;
//     this._movements = [];
//     this.locale = navigator.language;
//     console.log(`Welcome ${owner} thx for opening new account!`);
//   }
//   // Public interface
//   getMovements() {
//     return this._movements;
//   }

//   deposit(val) {
//     this._movements.push(val);
//   }
//   withdraw(val) {
//     this.deposit(-val);
//   }
//   _approveLoan(val) {
//     return true;
//   }
//   requestLoan(val) {
//     if (this._approveLoan) {
//       this.deposit(val);
//       console.log(`the Request for the loan: ${val} has accepeted`);
//     }
//   }
// }

// const adam = new Account('Adam Elimelech', 'ILS', 1111);

// adam._approveLoan(50);
// adam.deposit(50);
// adam.requestLoan(2250);
// adam._movements.push(555);
// console.log(adam);
// console.log(adam.getMovements());

// class Student extends Person {
//   universety = 'Udemy';
//   #studyHours = 0;
//   #course;
//   static numSubjects = 10;
//   constructor(fullName, birthYear, startYear, course) {
//     super(fullName, birthYear);
//     this.startYear = startYear;
//     this.#course = course;
//   }

//   intro() {
//     console.log(`Hello my name is ${this.fullName}`);
//   }
//   study(h) {
//     this.#makeCoffe();
//     this.#studyHours += h;
//   }
//   #makeCoffe() {
//     console.log(`i made you coffe!`);
//   }
//   get testScore() {
//     return this._testScore;
//   }
//   set testScore(score) {
//     this._testScore = score < 20 ? score : 0;
//   }
//   static printCurriculum() {
//     console.log(`There are ${this.numSubjects} subjects`);
//   }
// }
// const admon = new Student('Adam Elimelech', 1995, 2022, 'CS');

// admon.study(5);
// admon.study(5);
// console.log(admon);

////////////////////////
// Coding challenge #4

/*
  1. Re-create challenge #3 but this time using ES6
  classes: create an 'EVCl' child class of the 'CarCL' class;
  2. Make the 'charge' property private;
  3. Implement the ability to chain the 'accekerate' and
  'chargeBattery' methods of this class, and also update
  the 'brake' method in the Car class,They experiment with chaining

  DATA CAR 1: 'Rivian' going at 120 km/h, with a charge of 23%; 

 */
class CarCl {
  constructor(make, speed) {
    this.make = make;
    this.speed = speed;
  }
  accelerate() {
    this.speed += 10;
    console.log(`${this.make} has acclerate ,currect speed: ${this.speed}`);
    return this;
  }
  break() {
    this.speed -= 5;
    console.log(`${this.make} has breaked ,currect speed: ${this.speed}`);
    return this;
  }
  get SpeedUS() {
    const speedInMiles = this.speed / 1.6;
    console.log(`Speed in MI/H: ${speedInMiles}`);
  }
  set SpeedUS(speed) {
    this.speed = speed * 1.6;
    console.log(`Speed in KM/H: ${this.speed}`);
  }
}

class EVCl extends CarCl {
  #charge;
  constructor(make, speed, charge) {
    super(make, speed);
    this.#charge = charge;
  }
  chargeBattery(val) {
    this.#charge = val;
    console.log(this.#charge);
    return this;
  }
  accelerate() {
    this.speed += 20;
    this.#charge--;
    console.log(
      `${this.make} has acclerate ,currect speed: ${
        this.speed
      } with a charge of ${this.#charge}`
    );
    return this;
  }
}

const Rivian = new EVCl('Rivian', 120, 23);
console.log(Rivian);
// Rivian.SpeedUS;

Rivian.accelerate()
  .accelerate()
  .accelerate()
  .break()
  .chargeBattery(50)
  .accelerate();

// class Student extends Person {
//   universety = 'Udemy';
//   #studyHours = 0;
//   #course;
//   static numSubjects = 10;
//   constructor(fullName, birthYear, startYear, course) {
//     super(fullName, birthYear);
//     this.startYear = startYear;
//     this.#course = course;
//   }

//   intro() {
//     console.log(`Hello my name is ${this.fullName}`);
//   }
