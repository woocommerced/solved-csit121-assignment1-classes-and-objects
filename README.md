Download Link: https://assignmentchef.com/product/solved-csit121-assignment1-classes-and-objects
<br>
This assignment aims to provide you with some experience in writing codes using Java programming language that covers the following topics:

<ul>

 <li>Classes and Objects</li>

 <li>Interaction between Classes</li>

</ul>

<table width="732">

 <tbody>

  <tr>

   <td width="732"><strong> </strong><strong>Remember that: </strong><strong>1.         </strong><strong>All programs should be able to run on the lab’s computers. </strong><strong>2.         </strong><strong>You must put the following information on the header of each text and source file you will be submitting in this assignment:  </strong><strong>     Student’s full name:   </strong><strong>     Student’s ID:   </strong><strong>     Modification Date:  </strong><strong>     Purpose of this file (or program):   </strong><strong>3.         </strong><strong>Assignments that are not able to be compiled will result in zero mark given to the assignment. </strong><strong>4.         </strong><strong>You must only use the Java features that have already been covered in the lectures </strong><strong> </strong></td>

  </tr>

 </tbody>

</table>




<strong>TASKS: </strong>

This assignment will require you to design a set of classes that work together to simulate a police officer issuing a parking ticket. You are then required to write a Java application to demonstrate how the objects from these class interact. The description of each classes are given below.







<h2>The ParkedCar Class</h2>




This class is used to simulate a parked car at a parking lot. The class should contain the following attributes:




<ul>

 <li>The car’s make (example: Honda)</li>

 <li>The car’s model (example: Accord)</li>

 <li>The color of the car</li>

 <li>The car’s registration number</li>

 <li>The number of minutes the car has been parked</li>

</ul>

The class should have a constructor to initialize the make, model, color, and registration number with the values passed as parameters. The number of minutes should start with zero (0). There should be a set method to set number of minutes and a get method to retrieve the number of minutes.

The ParkingMeter Class




This class is used to simulate a parking meter. The class’s only responsibility is to set and know the number of minutes of parking that has been purchased by a car parked at the lot. The class will contain only one attribute:




 The number of minutes of parking time purchased

Include a default constructor to initialize the time to zero (0), a method to set the minutes purchased, and a method to retrieve the minutes purchased.

<h2>The ParkingTicket Class</h2>




This class is used to simulate a parking ticket issued by a police officer for a car that has parked illegally. The class should keep the details of:




<ul>

 <li>The illegally parked car. This should be declared as a ParkedCar object you have declared above.</li>

 <li>The amount of fine.</li>

 <li>The police officer who issue this parking ticket. This should be declared as a PoliceOfficer object (details below)</li>

 <li>A public class variable to represent the fine rate for the first hour and is initialized to RM150.00, a public class variable to represent the fine rate for additional hour and is initialized to RM50.00, and a public class variable to represent the maximum fine rate and is initialized to RM300.00.</li>

</ul>

The class should have a default constructor, a set method to assign a ParkedCar object, a set method to assign the PoliceOfficer object, a method to show the details of the ParkingTicket (which includes the ParkedCar details, the PoliceOfficer details and the amount of fine), and a method to calculate the amount of fine.




The method to calculate the amount of fine should take as parameter the number of minutes of parking time purchased by the car which is taken from the ParkingMeter object. The fine is calculated by first calculating the number of minutes the car is parked beyond the parking time purchased. The fine is RM150.00 for the first hour or part of an hour that the car is illegally parked, plus RM50.00 for every additional hour or part of an hour that the car is illegally parked. The maximum fine should be RM300.00.




<strong> </strong>

<h2>The PoliceOfficer Class</h2>




The PoliceOfficer class is used to simulate a police officer inspecting parked cars. The police officer will issue a parking ticket if a parked car is found to be illegally parked at a parking lot. This class keeps the following details about a police officer.




<ul>

 <li>The police officer’s name</li>

 <li>The police officer’s badge number</li>

</ul>

The class should implement a suitable constructor, set methods, and get methods.




<strong>The main application </strong>




Write another class to be the main application that simulate the interaction between all the classes above. Your application should simulate the following activities:




<ul>

 <li>A police officer sign up for duty. This will involve creating a PoliceOfficer If a ticket is issued when this officer is on duty, the details will be stated on the parking ticket issued. You may have more than one police officer but only one should be on duty at a time in this simulation.</li>

</ul>




<ul>

 <li>Creating ParkedCar This will involve creating several ParkedCar objects. You should make some of them are illegally parked and some are not. Use an array named parkingLot to keep all your ParkedCar objects. For each of the ParkedCar object, there should be a ParkingMeter object created to simulate the purchasing of the parking time. The ParkingMeter objects should be kept in another array named meters. The index of the arrays will be used to simulate parking lot and its parking meter. For example, if a ParkedCar object is stored at parkingLot[3] then its ParkingMeter will be stored in meters[3].</li>

</ul>




<ul>

 <li>Inspecting ParkedCar objects and ParkingMeter This is where the police officer will inspect all cars that are parked to check if they are illegally parked. A ParkingTicket will be issued (a ParkingTicket object is created) if a ParkedCar is found to be illegally parked. A ParkedCar is illegally parked when the parking time purchased by the car has expired. All ParkingTicket objects should be stored in an ArrayList.</li>

</ul>




<ul>

 <li>Displaying all ParkingTicket This will display a list of all ParkingTicket objects that have issued during the simulation.</li>

</ul>




Remember to include suitable exceptions handling in your program, write meaningful comments, and use meaningful variables and methods names. Take an effort to make your output presentable and easy to understand.




<strong><em>Assumptions: </em></strong>




<em>In a typical situation, a parking meter will usually show the time remaining and as time passes, the time shown on the meter will decrease. For the purpose of this simulation, you are not required to show this. You may assume that the value entered for the </em><em>ParkingMeter class is showing the exact number of minutes of parking time purchased. </em>

<em> </em>

<em>This is also the same with the number of minutes the car has been parked in the </em><em>Car class. In a usual situation, this should be increasing. However, for the purpose of this simulation, you may assume that the value stored in the variable is showing the number of minutes the car has been parked as of that time. </em>





