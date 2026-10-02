TripSplit Online
=================
Files:
1. AppsScript.gs - Google Apps Script backend
2. index.html - online frontend

SETUP
1. Create a blank Google Sheet.
2. Open Extensions -> Apps Script.
3. Replace the default code with AppsScript.gs.
4. Save.
5. Deploy -> New deployment -> Web app.
6. Execute as: Me.
7. Who has access: Anyone (or your preferred access setting).
8. Copy the /exec Web App URL.
9. Open index.html and paste the URL.
10. Create a trip. Data is stored in the Google Sheet.

IMPORTANT
- The current version uses a simple shared Web App endpoint.
- Anyone who has the endpoint URL may be able to write data. For private/family use, add authentication before public deployment.
- For multi-user production use, a user/Trip PIN or Google login should be added.
