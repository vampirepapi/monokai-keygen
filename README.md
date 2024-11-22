# monokai-keygen
a keygen for monokai pro.
## Manual Instructions - 

Creating the license
Monokai Pro requires an email to purchase a license, so we're going to need one here. I'm going to use a placeholder address: email@example.com.

Sublime Text 3 -
Take your email address and get the MD5 hash of it; you can use a website like https://www.md5hashgenerator.com/ for this. My test email comes out with 5658ffccee7f0ebfda2b226238b1eb6e or use https://monogen.vercel.app/.

Now, take the first 25 characters (so 5658ffccee7f0ebfda2b22623 for me), and insert a - after every 5 characters. You'll now have a valid license; in my case, it's 5658f-fccee-7f0eb-fda2b-22623.

Visual Studio Code -
To get it to work with VScode, you need to MD5 the extension UUID with the email you want to use and use the first 25 characters of the MD5 hash for VScode.

something like:

extension UUID = fd330f6f-3f41-421d-9fe5-de742d0c54c0
email = pouet@pouet.com
MD5 hash of: fd330f6f-3f41-421d-9fe5-de742d0c54c0pouet@pouet.com 
The serial number
11111-22222-33333-44444-55555
Take the string fd330f6f-3f41-421d-9fe5-de742d0c54c0 and add your email to the end of it. Then, take the MD5 hash of the resulting string. I come out with 0f2df3b3627abf1e80de8950a3d45d9e.

Now, take the first 25 characters (so 0f2df3b3627abf1e80de8950a for me), and insert a - after every 5 characters. You'll now have a valid license; in my case, it's 0f2df-3b362-7abf1-e80de-8950a.

Applying the license -
The instructions for applying the license are only available to paying customers, but looking at the code quickly revealed how to do it. Here are the instructions for both editors.

Sublime Text 3 - 
Open ST3 and ensure you have Monokai Pro installed. Then, open up the user preferences for the theme (Preferences > Package Settings > Theme - Monokai Pro > Settings - User). Copy this text into the file, with the placeholder values changed appropriately:

		{
			"email": "{add your email here}", //without curly braces
			"license_key": "{add your license key here}" //without curly braces
		}

Save the file and restart ST3, and you should see a thank you pop-up message. You are now running an activated theme.

Visual Studio Code
Open VS Code and ensure you have Monokai Pro installed. Then, press Ctrl+Shift+P to open the command palette. Search for Monokai Pro and select the option Monokai Pro - enter license. Then follow the prompts on-screen to enter your email and license key. You will then see a thank you pop-up message. You are now running an activated theme.

Hope it works for you!
