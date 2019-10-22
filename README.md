LBPets - A simple plugin for adding pets to your server
======
Updated to latest API. Click [here](https://www.mediafire.com/file/ayjklrh973efyff/LBPets_v1.0.0.phar/file)

## This plugin allows a user to add pets to their server. The commands are simple:

| Command | Sub Command | User | Params | Description |
|:-------:|:-----------:|:----:|:------:|:-----------:|
| `lbpets`  |   `give`   | `<name>` |  `ChickenPet, OcelotPet, PigPet, WolfPet`  | Spawns a pet |
| `lbpets`  |   `remove`  | `<name>` |    | Removes a player's pet |
| `lbpets`  |    `find`   | `<name>` |    | Finds a player's pet |

## The plugin can also be accessed by its API

```
$LBPets = Server::getInstance()->getPluginManager()->getPlugin('LBPets');

// Give a pet
$LBPets->givePet($user, $pet);

// Remove a pet
$LBPets->removePet($user);

// Find a pet
$LBPets->findPet($user);
```
