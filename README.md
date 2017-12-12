privacyIDEA Authentication module for the Benno Mailarchive
===========================================================

This plugin adds two factor authentication to the WebUI of
the Benno Mailarchive.
The second factor is managed and validated by privacyIDEA.

The Benno Mailarchive needs the email address of the user.
Thus privacyIDEA needs to return the email address of the
authenticated user. To do so, you need to configure an
authorizatoin policy in privacyIDEA which uses with 
``add_user_in_response``.

Configuration
-------------

An example config file is located in ``benno.ini.example``.
Copy and install it to ``/etc/privacyidea/benno.ini``.

To use this script, you need to add a symbolic link in
``/etc/benno-web/auth.d/`` which points to this script.


Dependencies
------------

The script depends on ``python-configobj``.

