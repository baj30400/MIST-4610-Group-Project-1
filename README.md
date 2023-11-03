# MIST-4610-Group-Project-1
## Team Name
29704 Group 7
## Team Members
1) Alex Kang @ALEXKANG1
2) Andy Kim @Andykim2003
3) Braden Johnson @baj30400
4) Jake Page @jtp38938
5) Justin Hozman @jch69018
## Problem Description
The problem scenario we are modeling is for an NBA organization. Player is a central piece that connects to many different entities in the data model. As players are paid to play games they create injury reports, contracts, and have statistics for every game they play in. The organization has many staff members who receive contracts just as players do to run the behind the scenes of the organization. The organization is also centralized around fans who are supporting the organization financially. Fans purchase merchandise as well as tickets in order to attend games. Our group wants to model the relationships between the different entities and input data for the attributes. We are creating queries on the data to receive beneficial information about the organization and discover optimal performance. 
## Data Model
Our data model is based on an NBA organization. The player entity represents the players on the team and includes information such as their position, height, and weight. Players get injured from time to time and can have multiple injuries over the course of their career. The injury report entity details the type of injury and the date of the injury as well as when the player is expected to recover. Players can play in many games and games are played by multiple players. Therefore an associative table is created which is PlayerGameStatistics. The associative table includes a player's statistics for a game which are statistics such as points, assists, rebounds, blocks and more. The game entity includes the opponent, venue, and score. 

Contracts are how players and staff are paid. The contract entity includes the salary, start, and end of the contract. A contract is paid out in multiple instances and so there are multiple financial transactions. Financial transactions include the amount, date, and type. Contracts are connected to two entities both through a one to one relationship. The two tables are PlayerContracts and StaffContracts. PlayersContracts will have playerID and contractID as its primary keys and StaffContracts will have staffID and contractID as its primary keys. Players can have many contracts over the course of their career but a contract can only be associated with one player. Staff can also have many different contracts but StaffContracts can only be associated with one staff member. The staff entity includes staffName, staffRole, department, and other information. 

Fans are the main customer for the organization and fans purchase merchandise. Fans can buy as much merchandise as they want and merchandise can be purchased by multiple fans. The fans table includes the name of the fan as well as their email, phone number, and date of birth. The merchandise table includes the item name and the category it belongs to as well as size, color, quantity, and price. The fan and merchandise table share a many to many relationship and create the associative table merchandise purchase. The associative table includes the fan and merchandise primary keys as its own primary keys and includes attributes such as buy price, quantity sold, payment method, and shipping address.

Fans also support the organization by attending games. Games are attended by many fans and fans can attend many games so an associative table is created called tickets. Tickets have the game and fan primary keys as its own primary keys. Attributes include price, purchase date, seat number, and more. The game is also played at an arena. An arena can have many different games played at the venue but a game can only be played at one arena. Arena includes attributes such as arena name, location, seating capacity, amenities, and more. 

<img width="639" alt="Screenshot 2023-11-03 at 2 07 57 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149821533/4b603184-f859-4ff1-b9a9-9b9ae72c3771">


## Data Dictionary

<img width="755" alt="Screenshot 2023-11-03 at 2 10 23 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149821533/c062e977-dbaf-4f9c-9df7-0a522478e6a9">

<img width="745" alt="Screenshot 2023-11-03 at 2 11 23 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149821533/3c1c8c5a-12f1-4173-a27a-72489aa8e4e3">

<img width="775" alt="Screenshot 2023-11-03 at 2 11 50 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149821533/51bf02cf-a55c-4c95-88a4-9b3555d5fa93">

<img width="754" alt="Screenshot 2023-11-03 at 2 12 53 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149821533/535bbc56-e953-405b-8ca2-b6908dc2b62a">

<img width="759" alt="Screenshot 2023-11-03 at 2 13 13 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149821533/1a77ae7b-198d-4050-a2d2-e518e97d31d1">




## Queries
- Query 1
  - <img width="809" alt="Screenshot 2023-11-03 at 2 12 57 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149818793/fc3889f5-c8c7-4ebb-a374-404fa339c39e">
  - Query 1 
- Query 2
  - <img width="661" alt="Screenshot 2023-11-03 at 2 17 55 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149818793/c983a7ad-9940-4dfc-a21f-ab7619f9fb76">
  -
- Query 3
  - <img width="540" alt="Screenshot 2023-11-03 at 2 20 08 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149818793/263a8e35-a0ac-4022-b529-fdb26cb3ab35">
  -
- Query 4
  - <img width="827" alt="Screenshot 2023-11-03 at 2 23 05 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149818793/ad4b2502-5991-49f0-bc06-b991004d3c0d">
  -
- Query 5
  - <img width="1440" alt="Screenshot 2023-11-03 at 2 35 52 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149818793/39b06be2-82b3-4980-ae0a-cbfb50d34019">
  -
- Query 6
  - <img width="1205" alt="Screenshot 2023-11-03 at 2 31 24 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149818793/bd0d7001-7d5e-4357-b850-412b9f36dd0c">
  -
- Query 7
  - 
  -
- Query 8
  - <img width="622" alt="Screenshot 2023-11-03 at 2 32 01 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149818793/52ca513c-e487-4109-a584-2cf0f3bfcea6">
  -
- Query 9
  - <img width="622" alt="Screenshot 2023-11-03 at 2 32 55 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149818793/89ff9db7-828f-4af4-983b-d4468e931ce8">
  -
- Query 10
  - <img width="621" alt="Screenshot 2023-11-03 at 2 39 11 PM" src="https://github.com/baj30400/MIST-4610-Group-Project-1/assets/149818793/b25ca164-d4b0-4e9d-8a13-bed4667846e9">
  -

## Database Information
- Name of the Database: ns_F2329704Group7
- Additional information: Each query listed above is marked in the database using stored procedures which can be called using the following format: CALL TP_Q1();
