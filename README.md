
# Office Attendance System (Group 24)

### Application Description: **Office Attendance System**

The **Tracking App** is a simple yet intuitive application designed to track and visualize the location data of users. The app allows users to monitor individual members' current locations, their previously visited locations, and the routes they have traveled. 

#### Key Features:
1. **Member List**: A user-friendly list of all members, each with the option to view their location details.
2. **Location Screen**: Displays the current location of a selected member along with a timeline view of visited locations. Users can see today’s location history or filter for past dates.
3. **Route Details**: Visual representation of routes between two visited locations, including details such as start and stop locations, total distance traveled, and total duration. Stops made for over 10 minutes are also highlighted.
4. **Dummy UI**: A simulated map interface that uses simple design elements (without Google Maps API) to represent user locations and routes.

This app is ideal for use cases like employee attendance monitoring, fleet management, or personal location tracking, and can be scaled to include real-time location services.


## Screenshots

![Screenshot_20240923_230451](https://github.com/user-attachments/assets/a0bd47b4-dda8-4284-b692-1a3385494289)


![Screenshot_20240923_230557](https://github.com/user-attachments/assets/1fbccbff-31f2-431e-b8e0-6fce7ca6ccd2)



## Explanation of code

1. MaterialApp:

This widget wraps the entire application. It provides navigation, routing, and theming features.
The app's title is "Location Tracker," and it's styled with a blue theme.

2. initialRoute: '/':

This defines the first screen the app loads, which in this case is the MemberListScreen.

3. routes:

The routes table defines the paths for navigation in the app.
The root path / is mapped to MemberListScreen().
The path /location is mapped to MapScreen(), and it expects a Member object passed through arguments when navigating to it.

4. pushNamed:

When navigating to the MapScreen, the Member object is passed as an argument. For example, you can use this code in MemberListScreen to navigate:
