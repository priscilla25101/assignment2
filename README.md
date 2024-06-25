The provided code defines a Flutter application with basic navigation features. Here is an explanation of the output and functionality:

### Application Overview:
- **Title:** Navigation Demo
- **Theme:** Primary color is blue.
- **Home Screen:** A `HomeScreen` widget that displays different screens based on user interaction.

### Main Components:

1. **Main Application (`MyApp`):**
   - Sets up the MaterialApp with a title and theme.
   - The home screen is set to `HomeScreen`.

2. **HomeScreen (`HomeScreen` Stateful Widget):**
   - **State Variables:**
     - `_selectedIndex`: Tracks the currently selected index of the bottom navigation bar.
     - `_screens`: A list containing instances of `SignInScreen`, `SignUpScreen`, and `CalculatorScreen`.

   - **State Methods:**
     - `_onItemTapped(int index)`: Updates `_selectedIndex` when a navigation item is tapped.

   - **Build Method:**
     - **AppBar:** Displays the title "Navigation Demo".
     - **Body:** Displays the screen corresponding to `_selectedIndex` from the `_screens` list.
     - **BottomNavigationBar:**
       - Contains three items (Sign In, Sign Up, Calculator) with corresponding icons.
       - Updates `_selectedIndex` when an item is tapped.
       - Highlights the selected item in amber color.
     - **Drawer:**
       - Contains a header and three list items (Sign In, Sign Up, Calculator).
       - Tapping on an item updates the `_selectedIndex` and closes the drawer.

### Expected Output:

- **Home Screen:**
  - Initially, the Sign In screen is displayed because `_selectedIndex` starts at 0.
  - The app bar shows the title "Navigation Demo".
  - The bottom navigation bar is present at the bottom with three items.

- **Bottom Navigation Bar:**
  - Three items are displayed: Sign In, Sign Up, and Calculator.
  - Tapping on any item updates the main content area to display the corresponding screen (Sign In, Sign Up, Calculator) and changes the selected item color to amber.

- **Drawer:**
  - Accessible via the app bar menu icon.
  - Displays a header "Navigation Drawer" and three list items: Sign In, Sign Up, Calculator.
  - Tapping on an item closes the drawer and updates the main content area to display the corresponding screen.

### Navigation Flow:
1. **Sign In (default):**
   - By default, the Sign In screen is displayed.
   - Tapping the Sign In icon in the bottom navigation bar or drawer doesn't change the screen but highlights the icon.

2. **Sign Up:**
   - Tapping the Sign Up icon in the bottom navigation bar or drawer switches the content area to the Sign Up screen.
   - The Sign Up icon is highlighted in the bottom navigation bar.

3. **Calculator:**
   - Tapping the Calculator icon in the bottom navigation bar or drawer switches the content area to the Calculator screen.
   - The Calculator icon is highlighted in the bottom navigation bar.
   - ![home](https://github.com/priscilla25101/assignment2/assets/164914474/71b46198-8dd6-4a29-a233-3e8092d8d0a7)


In summary, the application allows the user to switch between three screens (Sign In, Sign Up, Calculator) using either the bottom navigation bar or the navigation drawer. The currently selected screen is indicated by the highlighted item in the bottom navigation bar.
