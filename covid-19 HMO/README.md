# Covid-19 Patient Management System for Health Insurance Fund

## Overview
This project is a Covid-19 patient data management system designed for fund members of a large health insurance fund.  
Each fund member record includes personal details (full name, ID number, address, etc.) along with Covid-19-related data such as infection date (optional), recovery date (optional), and vaccination history.

## Features
- Manage fund member record: fetch all fund members, get the full personal details about the fund member, add a fund member, edit and delete.
- Add and update infection and recovery dates for each fund member.
- Vaccinations schedule management: add the required vaccinations to a fund member, along with the vaccination date and vaccine manufacturer. Each fund member has a maximum of 4 vaccines.

## Use Of Technologies
- Server side: C# .NET Core
- Client side: Angular, TypeScript
- Design libraries: Angular Material
- Database: SQL Server

## Installation
First clone the file to your local computer by the following command in the command line of the desired folder:
```bash
git clone https://github.com/shirabiton/Hadasim.git
```
### Server-side installation:
1. Open `WebApi.sln` file in Visual Studio.
2. Open the Package Manager Console (make sure the default project is `DataContext`)
3. Run the the following command to crate a migration:
```bash
add-migration <migration-name>
```
4. Update the database:
```bash
update-database
```
5. Run the WebApi project. Swagger UI will be opened automatically.

### Client-side installation:
1. Navigate to the `project` folder:
```bash
   cd project
```
2. Install dependencies:
```bash
   npm install
```
3. Start the Angular development server:
```bash
ng serve
```

## Assumptions
- We assume that each fund member can get sick with Covid-19 at most once

## How to use
From the home page, clicking on the 'Fund Members' button brings up a list of the full names of all fund members. You can search for a specific fund member by name in the search box. <br>
We will add a new fund member by clicking on the plus, adding a profile picture to a fund member is optional.<br>
Clicking on a specific member will bring us to his full details, <br>
Clicking on the icons at the bottom of the page will allow us to edit a fund member's details, delete a fund member or add vaccinations to him.<br>
At each stage, clicking on the logo at the top of the page will navigate to the home page.<br>


## A Visual Guide
Home Page:<br><br>
![Home Page](screenshots/home.png)
<br><br>
List of fund members:<br><br>
![List of fund members:](screenshots/members-list.png)
<br><br>Add a fund member:<br><br>
![Add a fund member](screenshots/add-member.png)
<br><br>
Fund member details:<br><br>
![Fund member details](screenshots/member-details.png)
<br><br>
Update fund member details:<br><br>
![Update member details](screenshots/update-member.png)
<br><br>
Adding a vaccine to a fund member:<br><br>
![Adding a vaccine to a fund member](screenshots/add-vaccine.png)
<br><br>
