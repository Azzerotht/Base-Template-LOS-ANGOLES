lien de téléchargement : https://www.mediafire.com/file/tg2sw3kze39dvq0/TEMPLATE_LA_0.0.2.zip/file

Pour les lignes MYSQL dans les fxmanifest

Rempalcer **"@oxmysql/lib/MySQL.lua",**  par **"@es_extended/modules/MySQL/lib/MySQL.lua",**


Si vous rencontrez des problème rendez vous sur https://discord.gg/ESUsR5Hw


Dans un fichier qui utilise une bdd 

Par example ici :

```fx_version 'cerulean'
game 'gta5'
lua54 'yes'
description 'Allows Players to buy & sell vehicles'
version '1.0'
legacyversion '1.9.1'

shared_script '@es_extended/imports.lua'

server_scripts {
    '@oxmysql/lib/MySQL.lua',
    '@es_extended/locale.lua',
    'locales/*.lua',
    'config.lua',
    'server/*.lua'
}

client_scripts {
    '@es_extended/locale.lua',
    'locales/*.lua',
    'config.lua',
    'client/*.lua'
}

dependency 'es_extended'

export 'GeneratePlate'

Rempalcer "@oxmysql/lib/MySQL.lua",  par "@es_extended/modules/MySQL/lib/MySQL.lua",

server_scripts {
    '@es_extended/modules/MySQL/lib/MySQL.lua',
    '@es_extended/locale.lua',
    'locales/*.lua',
    'config.lua',
    'server/*.lua'
}
