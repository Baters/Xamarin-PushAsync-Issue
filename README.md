# Xamarin-PushAsync-Issue
Using Xamarin Forms I find when following these instructions I find PushAsync stops working. It apps to be linked to changing the App.MainPage object. I need to understand what I am doing wrong. Any help is much appreciated.

Application overview
---------------------------
Separated into two areas, logon and main application. On startup the App.MainPage is set to a Navigation page containing ContentPage to capture username and password. When the user clicks Next another logon page is displayed which could be used to capture three random letters from a memorable word orr phrase. Once the user completes this page and clicks Logon the App.MainPage is updated to a new MasterDetailPage containing the Menu and the welcome page. 

Issue
-----
What I'm finding is after I've logged on and see the welcome page, if I click the Logout button on the menu and am brought back to the initial Logon screen when I click Next nothing seems to happen.

Steps to reproduce
------------------
1. Start application
2. On Logon (1 of 2) page click "Next Page"
3. On Logon (2 of 2) page click "Logon"
4. On Welcome page click "Menu"
5. Click "Logout"
6. Back on the Logon (1 of 2) page click "Next Page" again and even though you can debug through the page isn't displayed.

