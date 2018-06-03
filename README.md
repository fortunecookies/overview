# Introduction to FortuneCookies
FortuneCookies is a game of art and luck on Ethereum. Each FortuneCookie is a collectible good luck charm that contains a surprise! Players collect and trade FortuneCookies to maximize their GoodFortune, a form of digital luck that exhibits special powers.

FortuneCookies are produced in limited edition batches designed in collaboration with a unique artist. Everything from the design of the charm and the surprise inside, to the number of FortuneCookies produced, are part of the artist's intended experience. When you own a FortuneCookie, you actually own the digital rights to the associated art. Crack one open to see for yourself!

FortuneCookies batches are sold during official Bake Sales, which will be pre-announced on official FortuneCookies Twitter, Medium, and Telegram accounts at least a week prior. Batches are limited edition, so when they're gone they're truly gone – no more reprints can ever be made. Visit the [Official Bake Sale](www.fortunecookies.io/bakesale) to buy your FortuneCookie. If the Bake Sale is closed, FortuneCookies may be available for resale at popular collectibles exchanges like [RareBits](www.rarebits.io), [SuperRare](www.superrare.co), or [OpenSea](www.opensea.io).

FortuneCookies are secured by Ethereum. Technically, FortuneCookies are ERC721 tradeable tokens on the Ethereum blockchain (see ERC721: Non-Fungible Tokens). Because your FortuneCookies live on Ethereum, your GoodFortune will last for generations.

## Table of Contents
1. Collect Digital FortuneCookies
   1. The Charm    
   2. The Surprise    
   3. The Batch    
   4. The Bake Sale
2. Earn GoodFortune on Ethereum
   1. Your GoodFortune Score   
   2. The GoodFortune Formula   
           1. Fixed Attributes         
           2. Gameplay Multipliers          
   3. The GoodFortune API    
   4. The GoodFortune Oracle   
3. Spread Good Fortune in the World
   1. Artist Compensation   
   2. FortuneCookies Foundation   
   3. Community Culture   

## Collect Digital FortuneCookies
FortuneCookies are collectible charms with a surprise.

### The Charm
The charm is the exterior shell of the FortuneCookie, and contains the surprise hidden inside. All charms are the same for a whole batch, which makes it easy to associate your FortuneCookie with a batch when it's in your wallet – since the charm also functions as your collectibles icon.

### The Surprise
The surprise is the goodness hidden inside your FortuneCookie that reveals itself to the player that opens the FortuneCookie for the first time. We achieve this by using your Ethereum address to generate pseudorandomness, which assigns you a resultant surprise from the available batch. Unlike regular fortune cookies, FortuneCookies surprises are actually made-for-you.

### The Batch
FortuneCookies Batches are limited edition releases that can produce anywhere between 1 and 1 million new FortuneCookies. Batches are the main grouping of FortuneCookies in the game; FortuneCookies from the same Batch have the same Charm – and they usually share similar surprises. Players are restricted to holding only 1 FortuneCookie from each batch at a time.

Batches are designed in collaboration with an artist. The entire experience of the batch, from the number of FortuneCookies produced, to the charm and the surprise hidden inside, are the vision of the artist.

### The Bake Sale
Bake Sales are official FortuneCookies events when new FortuneCookies are sold to the public. Most Bake Sales will occur on our website, however some may occur offline or in person for special occasions. Bake Sale types include:
* Reverse Auction: fixed quantity; high > low variable price; sold sequentially.
* Vanilla Auction: Use cases include time-based drip auction (like CryptoKitties), single auction
* Dutch Auction: 
* Reverse Dutch Auction:
* Flash Sale: fixed quantity; fixed price; parallel sales, first come first served until gone.
* Buy Now: Can be applied to any sale; a price that is above current market rate and allows you to purchase the Next FortuneCookie.

View the [Bake Sale](www.fortunecookies.io/bakesale).

## Earn GoodFortune on Ethereum
Fortune as a positive attribute. Many cultures believe that luck and good fortune are attributes that a person can possess. We wanted to make this a literal reality, so we made GoodFortune an attribute on Ethereum.

### Your GoodFortune Score

GoodFortune is a form of public reputation for an Ethereum address. Because FortuneCookies live on the public Ethereum blockchain, their ownership can be publicly tracked. 

Publicly verifiable. GoodFortune is secured by Ethereum, so it is pub.
Luck that Follows You. Silos suck. Because your GoodFortune is 

If you care about the details of how your GoodFortune score is calculated, continue reading. If not, jump to "Spread Good Fortune in the World."

### The GoodFortune Formula
A player's GoodFortune is calculated by totaling the GoodFortune of their FortuneCookies. 

```GoodFortune(player) = sum((GoodFortune(FortuneCookie1)), (GoodFortune(FortuneCookie2)), ...)```

The amount of GoodFortune possessed by an individual FortuneCookie is determined by a combination of fixed and variable   attributes.

(FortuneCookieID)^(sqrt/FortuneCookieID)*

#### Fixed Attributes
Fixed and determined during the production of the batch.
* FortuneCookie ID: Unique FortuneCookies number. The first FortuneCookie produced will be #1. 
```(LastFortuneCookieID-FortuneCookieID)^2 <- or what curve do we want to use?```
* Batch: Overall batch ID number. The first batch produced will be #1. (Max value = 1) ```(LastBatchID-BatchID)^2```
* Rarity: (1/Batch Quantity) (Max value = 1)
* Sequence: ( ( ( BatchLast - FortuneCookieID ) / ( Range ) ) ) -- does this fail when it's the last cookie in the batch? What value should we assign or exception should we set?

#### Gameplay Multipliers
Behavioral; determined by gameplay.
* Sale Price: (std deviations from the mean) is the multiplier. (( or should this be last sale price? - it would be more realtime and punishing ))
* Change in Price: what has the price done
* Initial Owner GoodFortune Multiplier: XOXO !! The GoodFortune Multiplier !! XOXO When you buy FortuneCookies from Official Bake Sales, we offer a bonus incentive for our loyal players. We reserve the right to refuse transactions from any address choose, especially if we beileve it to be an aggregation service.
  * MVP - 25%: Determine the tiers
  * 25% - 50%: Determine the tiers
  * 50% - 75%: Determine the tiers
  * 75% - 100%: Determine the tiers
* Initial Owner Public Tweet: One time opportunity during the bake sale. (+10% multiplier)
* Previous Owners: 1.05^n // note: cost is 3.5% to exchange owners, so net 1.5%

>#### The GoodFortune API
>We offer simple a simple API to request information about a FortuneCookies player address. Our services cache blockchain information, making it easier to use when you need it. Easily get FortuneCookies or get GoodFortune balance for a player address. Learn more about [The GoodFortune API] 
>
>GetFortuneCookies() returns an array of the FortuneCookies owned by an
>
>GetGoodFortune() returns the total GoodFortune possessed by a player address
>
>#### The GoodFortune Oracle
>The GoodFortune Oracle is a smart contract on Ethereum that serves two important functions. First, it contains the official >formula for calculating GoodFortune the calculation for determining the amount of GoodFortune a FortuneCookie has, as well as >contains pointers to every official Batch contract

## Spread Good Fortune in the World
The Fortune Friends are committed to spreading good fortune, both digitally and IRL. It's our mission to use new technology as a powerful force of change, empowerment, and self-organization.

### Artist Compensation
We fairly compensate artists with between 10-20% of every sale, and 1.25% of every resale.

### FortuneCookies Foundation
We donate 10% of every sale to the FortuneCookies Foundation, a non-profit committed to spreading good fortune by investing in social impact bounties that matter to our community. Submit an idea at [FortuneCookies Foundation](http://fortunecookies.foundation). What change will you bounty?

### Community Culture
We want to promote a fun, open cult-ure. We value creativity, positivity, change, boldness, fun, and play. 
