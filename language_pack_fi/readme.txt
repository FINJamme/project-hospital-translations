@@ -0,0 +1,48 @@

What do the data look like?
The localization table is saved in plain text (XML) files, organized into different categories that make sense, for example:


    Texts in the menu and main user interface
    Medical terms - diagnoses
    Medical terms - examinations
    Texts for tutorials and campaign
    ...
    Names and descriptions of objects you can build


This will allow more people to translate one language.
The game directly reads these XML files, so it's possible to test the changes in the game without sending the files to the developers and waiting for a new version.

File heading
============
This is an example for Czech. Each file has to have a unique ID (change language code!). Values that need to be filled in each file are the language code in lower case (like en, fr, pt_br etc) and localized name (that's what will show in game).
Feel free to add you name to the list of contributors for any file you've made changes to!

<Database>
    <GameDBStringTable ID="LOC_CZ_ACHIEVEMENTS">
        
        <LanguageCode>FI</LanguageCode>
        <LanguageNameLocalized>Suomi</LanguageNameLocalized>

        <Contributors>
            <Name>Jamme</Name>
        </Contributors>


Some examples of the texts
==========================

    <GameDBLocalizedString>      <LocID>PERUUTA</LocID>                    <Text>PERUUTA</Text>  </GameDBLocalizedString>

    <GameDBLocalizedString>      <LocID>AMMATTI_LÄÄKÄRI</LocID>         <Text>Lääkäri</Text>  </GameDBLocalizedString>
    <GameDBLocalizedString>      <LocID>AMMATTI_SAIRAANHOITAJA</LocID>          <Text>Sairaanhoitaja</Text>  </GameDBLocalizedString>

    <GameDBLocalizedString>      <LocID>DIA_FLUNSSA1_KUVAUS</LocID>      <Text>Flunssa on yleinen hengitystieninfektio. Aikuisilla se voi kehittyä keuhkokuumeeksi, lapsilla taas kurkunpääntulehdukseksi tai korvatulehdukseksi.</Text>  </GameDBLocalizedString>


There are some formatting options available:
New line: \n 
Bold/italics:

    <![CDATA[Now <b><i>do something</i></b>.\nThis is on the next line.]]>
    <GameDBLocalizedString>      <LocID>AMMATTI_ORTOPEDI</LocID>         <Text>Ortopedi</Text>  </GameDBLocalizedString>    
