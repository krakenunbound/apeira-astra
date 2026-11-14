# Apeira Astra

An original science-fiction ruleset for [Kraken VTT](https://github.com/krakenunbound/kraken-vtt).

Small crews, cold reaches, and salvage law. Roll **2d6** plus a skill and a characteristic against **8**. The margin is the **Effect**. Armour soaks damage. There are no levels: experience buys skills and characteristics, and a **Mark** teaches a trick from your Path.

This repository is the books: the Crew Handbook, the Threat Dossier, *Salvage Rights*, and the one-session job *A Lamp in the Rock*. The dice engine stays in Kraken (`shared/astra`).

## What's in the box

- **Crew Handbook.** Origins, Paths, Marks and tricks, tasks, combat, vacuum, ships, and the gear a port will sell.
- **Threat Dossier.** People you can hire or cross, machines, creatures, a salvage roll, and six jobs ready to run.
- **Salvage Rights.** A first adventure, two sessions, aboard the freighter *Kestrel's Due*.
- **A Lamp in the Rock.** One session. Two stamps on one claim, a living passenger, and a case that should not be spun.

Nothing here is drawn from Traveller, Ringworld, Starfinder, or any other published science-fiction game. The setting, names, rules text, and pictures are original.

## Use it in a Kraken checkout

Kraken builds these files into the books it reads. From a checkout of Kraken VTT:

1. Copy the `apeira-astra` folder from this repo over `games/apeira-astra` in the checkout.
2. In `scripts/build-content.mjs`, import the adventure and add it to the module list:

```js
import { LAMP_IN_THE_ROCK } from "../games/apeira-astra/lamp-in-the-rock.mjs";
```

and include `LAMP_IN_THE_ROCK` in the `modules` array next to `SALVAGE_RIGHTS`.

3. Build the books:

```
node scripts/build-content.mjs
```

4. Start Kraken from that checkout, make a campaign with the ruleset **Apeira Astra**, and activate the Crew Handbook, the Threat Dossier, and the adventure you want to run.

A release install of Kraken ships its own copy of the books. This repo is the newer text. It shows up when you run the checkout you copied it into.

## License

Copyright © The Kraken. The rules text, setting, names, and art in this repository are original and may be shared and played with Kraken VTT. Apeira Astra is not affiliated with or endorsed by any other game's publisher.
