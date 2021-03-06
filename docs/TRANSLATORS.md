Translator Info
---------------

If you like phpPgAdmin6, then why not translate it into your native language?

There are quite a large number of strings to be translated.  Partial
translations are better than no translations at all, and a rough guide is that
the strings are in the order from most important to least important in the
language file.  You can ask the developers list if you don't know what a
certain string means.

We tried keeping translation easy in phpPgAdmin6 by using ONLY the UTF-8 charset.
Make sure to always work on UTF-8 files when creating a new translation or
editing an existing one.

To Create a new translation:

1. Go to the lang/ subdirectory

2. Copy english.php to yourlanguage.php

3. Update the comment at the top of the file.  Put yourself as the language 
   maintainer. Edit the 'applang' variable and put your language's name in it,
   in your language.
   Edit the 'applocale' and put your language code according to the standart:
     http://www.ietf.org/rfc/rfc1766.txt

   Basicaly, you just need to put your language code [1] and optionnaly country
   code [2] separated by a '-'. As instance for french canadian, it is: fr-CA
     [1]: http://www.w3.org/WAI/ER/IG/ert/iso639.htm
     [2]: http://www.iso.org/iso/country_codes/iso_3166_code_lists/country_names_and_code_elements.htm

4. Go through as much of the rest of the file as you wish, replacing the
   English strings with strings in your native language.

At this point, you can send the yourlanguage.php file to us and we will take
care of testing and recoding the translation.  Please only do that if you 
find the rest of these steps too difficult.

5. To add your language to phpPgAdmin6, edit the lang/translations.php file
   and add your language to the $appLangFiles array.
   Also, add your language to the $availableLanguages array for
   browser auto detection.

6. Send your contribution to us.  We need the lang/translations.php entry as 
   well as the lang/yourlanguage.php file.  Email to the developers list:
     phpPgAdmin6-devel@lists.sourceforge.net

7. There exists a tool named 'langcheck' in the lang/ directory.  To run it,
    just type 'php langcheck <language>'.  It will give you a report about
    which strings are missing from your language file and which need to be
    deleted.

Thank you for your contribution!  You have just made phpPgAdmin6 accessible
to thousands more users!
