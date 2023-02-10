## Braille*Rap*

# !!!!!!!!!!! This is for BrailleRapSP !!!!!!!!!

Emboss Braille with a BrailleRapSP! This is a modified version of original [ArthurSW](https://github.com/arthursw) work https://github.com/arthursw/BrailleRap to handle the Braille printer BrailleRapSP. The main modification is that ArturSW version use a motor for the Z axis, BrailleRAP-SP use an electro-magnet and don't have a Z axis. So the G-CODE is slightly different, and not portable !

Thanks to [Avinash Pudale](https://github.com/AvinashPudale) the application now support
indian devnagari languages  (hindi,marathi,nepali) 
Emboss Braille with BrailleRapSP!



BrailleRAPSP repo is here https://github.com/BrailleRapSP/BrailleRapSP



### Contribution

You can modify and/or add braille language files (braille6.js, braille6india.js, braille8new.js, braille8old.js, devnagrinumbers.js).
 
 edit devnagrinumbers.js for numbers and custom indices

Those are javascript files, not JSON, to be able to include them in the index.html file when working offline without a server.

Any new language file respecting this format will be automaticaly taken into account. The name of the language must contain '6 dots' if it is based on 6 dots, '8 dots' if based on 8 dots.


# 📋 About this fork

Simplification du HTML

Correction du bug relatif aux caractères spéciaux en majuscule empêchant l'écriture. Dans le fichier [script.js](https://github.com/Vntoine/BrailleRap/blob/master/script.js) version [fe7cdf4](https://github.com/Vntoine/BrailleRap/commit/fe7cdf4b6f68d73ebd40c8e468109b5be894855a#diff-ed3ee7e0beea2498ff3b8ca85973d122fc6fa3d585d62b5807ec034d0cf076b3) : 
```
# Modification de l'expression régulière pour inclure les caractères suivants : "ÀÂÇÈÉÊËÎÏÔÙÛÜ".
# La fonction toLowerCase() de JavaScript renvoie correctement la minuscule correspondante,
  l'ajout du préfixe se fait sans problème !
```
