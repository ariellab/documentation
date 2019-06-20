======================
Synchronizing with iOS
======================

Calendar
--------

#. Open the settings application.
#. Select Mail, Contacts, Calendars.
#. Select Add Account.
#. Select Other as account type.
#. Select Add CalDAV account.
#. For server, type ``example.com/remote.php/dav/principals/users/USERNAME/``
#. Enter your user name and password.
#. Select Next.
#. If your server supports SSL, iOS may still give you a "Cannot Connect Using SSL" pop-up because the initial server address you provided will have been carried to the Advanced Settings screen, and you must next specify port 443, and trim the server address back down to just the domain part. Here's how:

   -  Select Cancel on the "Cannot Connect Using SSL" pop-up error message.
   -  Select OK on the "Calendar Account Unable to verify account information." pop-up message that will follow.
   -  Select Advanced Settings.
   -  Verify that the "Use SSL" toggle is set to ON.
   -  Enter the number 443 in the Port data entry field.
   -  Verify that the server address is prefixed with "https", not "http".
   -  Go back to account information by selecting <CalDAV in in the top left corner.
   -  Edit the Server field so that only your domain is provided, "example.com".
   -  Select Save.
#. If your server does not support SSL, or your iOS device is unable to verify the account information you provided, try the
   following steps:

   -  Select OK.
   -  Select Advanced Settings.
   -  If your server does not support SSL, make sure "Use SSL" is set to OFF.
   -  Enter the number 80 in the Port data entry field.
   -  Go back to account information and select Save.

When successful, you will see a series of checkmarks appear to the right of the data fields of the CalDAV account information, the form will close, and your calendar data will begin syncing and become visible in the Calendar application.


Contacts
--------

#. Open the settings application.
#. Select Mail, Contacts, Calendars.
#. Select Add Account.
#. Select Other as account type.
#. Select Add CardDAV account.
#. For server, type ``example.com/remote.php/dav/principals/users/USERNAME/``
#. Enter your user name and password.
#. Select Next.
#. If your server supports SSL, iOS may still give you a "Cannot Connect Using SSL" pop-up because the initial server address you provided will have been carried to the Advanced Settings screen, and you must next specify port 443, and trim the server address back down to just the domain part. Here's how:

   -  Select Cancel on the "Cannot Connect Using SSL" pop-up error message.
   -  Select OK on the "Calendar Account Unable to verify account information." pop-up message that will follow.
   -  Select Advanced Settings.
   -  Verify that the "Use SSL" toggle is set to ON.
   -  Enter the number 443 in the Port data entry field.
   -  Verify that the server address is prefixed with "https", not "http".
   -  Go back to account information by selecting <CardDAV in in the top left corner.
   -  Edit the Server field so that only your domain is provided, "example.com".
   -  Select Save.
#. If your server does not support SSL, or your iOS device is unable to verify the account information you provided, try the
   following steps:

   -  Select OK.
   -  Select Advanced Settings.
   -  If your server does not support SSL, make sure "Use SSL" is set to OFF.
   -  Enter the number 80 in the Port data entry field.
   -  Go back to account information and select Save.

When successful, you will see a series of checkmarks appear to the right of the data fields of the CardDAV account information, the form will close, and your calendar data will begin syncing and become visible in the Contacts application.

If it's still not working, have a look at the `Troubleshooting Contacts & Calendar`_
guide.

.. _Troubleshooting Contacts & Calendar: https://docs.nextcloud.org/server/14/admin_manual/issues/index.html#troubleshooting-contacts-calendar
.. TODO ON RELEASE: Update version number above on release
