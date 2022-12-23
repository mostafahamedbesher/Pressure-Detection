# Pressure-Detection


## Description

* Pressure-Detection Function Is To Detect High Pressure in a Plane Cabin. If High Pressure Detected , It Raises Alarm 
  Which Is Turnning On Led For 60 Seconds.
* Design of this project based on UML Diagrams.

## Project Design

* To Efficiently Design This System I Go Through These Design Stages : 
  * Case Study
  * Design Method
  * Requirements
  * Space Exploration/Partioning
  * System Analysis
  * System Design
  
 1- Case Study
 
  * A Client Expects To Deliver The Software of The Following System :
  
    * Specifications :
      * Detection System which Informs The Crew Of a Cabin With An Alarm When Pressure Exceeding 20 Bars In The Cabin
      * The Alarm Duration Equals 60 Seconds
      * Keep Track Of The Measured Values 
      
    * Assumptions :
      * The controller set up and shutdown procedures are not modeled
      * The controller maintenance is not modeled
      * The pressure sensor never fails
      * The alarm never fails
      * The controller never faces power cut
      * Versioning  The ”keep Track Of Measured Value”  Option is not Modeled in The First Version Of The Design
      
  2- Design Method :
  
    * I used Water Fall Design Method
    
    
![waterfall](https://user-images.githubusercontent.com/77936621/209389329-90c58181-5aa6-4fca-973b-521305edd2ee.png)


  3- Requirements :
  
    * Requirement Diagram :
    
![requirement](https://user-images.githubusercontent.com/77936621/209389537-8e7beac7-e0d7-44ab-a58c-4e9115e23e17.png)


  4- Space Exploration/Partioning :
  
    * Used STM32F103C6 SOC Which Based On Arm Cortex–M3 Micro Processor Which Specifications Are :
    
      * ARM 32-bit Cortex™-M3 CPU Core 72 MHz maximum frequency,1.25 DMIPS/MHz (Dhrystone 2.1) performance at 0 wait state memory access
      
      
  5- System Analysis :
  
    * Use Case Diagram

![use_case_diagram](https://user-images.githubusercontent.com/77936621/209390505-e201e430-9e68-4258-b9f7-7a9274534e93.png)

      * Use Case Diagram function is to inform the client Of what the system main functions and define system Boundary With some level of abstraction of system details
      
      
  6- Activity Diagram :
  
  
![activity_diagram](https://user-images.githubusercontent.com/77936621/209391003-5a364036-54f3-4f57-b9b1-6a08d315524e.png)


      * Activity function is to show the relations Between main functions of the system And describe the work flow of the system.
      
      
   7- Sequence Diagram : 


 ![sequence_diagram](https://user-images.githubusercontent.com/77936621/209391208-19ae7fa5-625a-4f77-91c1-a9fffb686bb8.png)

      * Sequence Diagram is an interaction diagram that details how operations are carried out and Shows What messages are sent and when.
      * Sequence diagrams are organized according to Time.
      
   8-  System Design : 
   
      * Block Diagram : 
      
      
![block_diagram](https://user-images.githubusercontent.com/77936621/209391409-eb0a5f41-768d-46cc-84de-9be073bf0c69.png)


      I used here multiple modules in block diagram, one module For pressure sensor, one for alarm actuator and the last one
      For main algorithm of the system which controls it.
      
      * State Machine Diagram : 
      
        * For pressure sensor module :
        
 ![state_diagram_pressure_sensor](https://user-images.githubusercontent.com/77936621/209391727-e49236dd-5373-457a-bdad-6c104fbe8f21.png)
 
        * For alarm actuator module : 
        
        
![state_diagram_alarm](https://user-images.githubusercontent.com/77936621/209391794-f6183270-5812-4570-b460-c4b9f2ef5d13.png)

  
        * For main algorithm Module :
        
        
![state_diagram_algorithm](https://user-images.githubusercontent.com/77936621/209391876-8cc53f74-c37f-4866-a161-a53511653231.png)

      * Simulation : 
      
      
![simulationtrace_fromttool](https://user-images.githubusercontent.com/77936621/209391961-9b49f864-7664-461c-a71c-d1265ca94ae1.png)



## Proteus Simulation :

* When pressure > 20 bars , alarm started
* Pressure in simulation equals 26 bars

![simulation_alarm_on](https://user-images.githubusercontent.com/77936621/209392190-fffb6c40-dc4a-4ac9-a93f-37781efe33a9.png)

* When pressure <= 20 bars, alarm stopped
* Pressure in simulation equals 13 bars

![simulation_alarm_off](https://user-images.githubusercontent.com/77936621/209392308-f89b39d9-5cb4-498d-8ff1-751663f0b4d4.png)





    
    


    
      
      









  
