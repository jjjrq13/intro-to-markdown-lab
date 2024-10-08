# What is the Perfect Old Fashioned and How is it Made?

![garnish being put in a spirit forward cocktail](./assets/Old%20Fashioned/Old-Fashioned.jpg)

An Old Fashioned is probably one of the oldest cocktails in the world, but to say that "THIS" is the right way to make it is very subjective. Different parts of the country, let alone the world, have their own ideas on what the perfect Old Fashioned is and how to make it. To make an Old Fashioned, all you need are four simple ingredients:

1. Whiskey
2. Sugar
3. Bitters
4. Garnish
5. Ice

Nothing more, nothing less. This combination gives whiskey lovers everywhere a cocktail they can enjoy.

You might think this is a guide to making the perfect Old Fashioned, but it's actually a guide on how to build one while experimenting and understanding what each ingredient does so you can find the perfect version for your palate. The best part of that is we'll build it using Javascript.

```js
// Lets start building or perfect old fashioned
const myPefectOldFashioned = {};
```

## Whiskey Rye or Bourdon?

Okay guys, this is the question that has affected the general public for years. before we behind lets just make one thing clear... When you ask a brtender for an old fashion a good bartender will grab bourdon and start making you the drink. a GREAT bartender will ask you if you **_Rye or Bourbon?_**

### Bourbon

There are 5 rules to what bourdon is but we will keep it simple here. Its a whikey made of atleast 51% corn, aged in new charred oak barrels, made in **MERICA** & bottled at atleast 40% alcohol.

Typical flavor profiles of bourbon are:

-   Sweet Vanilla
-   Cinnamon & Oak
-   Fruits
-   Caramel
-   Nuts

### Rye

On the other hand has to be made of atleast 51% Rye grain and aged in new charred oak barrels.

Typical flavor profiles of rye whiskey are:

-   spicy
-   fruity
-   grain
-   earthy
-   dry

Check out this [Peoples Bourbon](https://www.peoplesbourbonreview.com/bourbons/common-descriptive-words-for-bourbon.aspx) page to find a whiskey by flavor keywords. Are any of these available in your liquor store? Which one would you choose for your perfect Old Fashioned? Is there a rye or bourbon you already love that you know would work really well for your drink? Pick one and add it to our selection.

Here is mine:

```js
// use this object to add a whiskey to your cocktail. How will you add it?
const whiskey = {
    rye: [
        {
            name: 'WhistlePig 10 Year Rye',
            proof: 100,
            flavorProfile: ['Spicy', 'Oak'],
            yearsAged: 10,
        },
        {
            name: 'High West Double Rye',
            proof: 92,
            flavorProfile: ['Pepper', 'Caramel'],
            yearsAged: 2,
        },
        {
            name: 'Sazerac Rye',
            proof: 90,
            flavorProfile: ['Spicy', 'Vanilla'],
            yearsAged: 6,
        },
        {
            name: "Michter's 10 Year Rye",
            proof: 92.8,
            flavorProfile: ['Rich Spice', 'Oak'],
            yearsAged: 10,
        },
        {
            name: 'Old Forester Rye',
            proof: 100,
            flavorProfile: ['Pepper', 'Dark Chocolate'],
            yearsAged: 4,
        },
    ],
    bourbon: [
        {
            name: 'Buffalo Trace',
            proof: 90,
            flavorProfile: ['Vanilla', 'Oak'],
            yearsAged: 8,
        },
        {
            name: 'Woodford Reserve',
            proof: 90.4,
            flavorProfile: ['Caramel', 'Dried Fruit'],
            yearsAged: 7,
        },
        {
            name: "Maker's Mark",
            proof: 90,
            flavorProfile: ['Sweet', 'Vanilla'],
            yearsAged: 6,
        },
        {
            name: 'Four Roses Single Barrel',
            proof: 100,
            flavorProfile: ['Cherry', 'Cinnamon'],
            yearsAged: 7,
        },
        {
            name: 'Eagle Rare',
            proof: 90,
            flavorProfile: ['Toffee', 'Oak'],
            yearsAged: 10,
        },
    ],
};
```

//My pick
const myPerfectOldFashioned = { 
    whiskey: 
        { name: "Michter's 10 Year Rye", proof: 92.8, flavorProfile: ['Rich Spice', 'Oak'], yearsAged: 10, ounces: 2 } 
};


## Sugar

When adding sugar to an Old Fashioned, there are two ways to do it: by adding sugar directly from a bag or using a syrup. You can use white sugar or Demerara sugar, but we’ll focus on these two since they are the most commonly used in the drink.

-   **White Sugar**: Pure sweetness. Everything and anything else has been stripped away, leaving only refined sweetness.

-   **Demerara Sugar**: Minimally processed with large, amber-colored crystals and a slight molasses flavor, giving it a unique texture and taste.

> if anyone ever tells you that uou can use setiva, splenda or any artificial sugar send them to therapy and call the cops beause that one unforgivable crime

in 1843 a wonderful man invented the sugar cube and in the world of great drinks every place that calls itself a cocktail bar will have them. If you have a bag of sugar in your home think of a sugar cube as a teaspoon. Either way you can use one or the other. If you want to use a simple syrup you can add anywhere from 1/8oz to 3/4oz of syrup.

> Want to make a simple syrup at home?
>
> > Mix 1 part Sugar to 1 Part Water until fully disolved

```js
//To Syrup or to Cube that is the question?

const sugarCube = {
  white: [1, 2, 3, 4, 5],
  demarara: [1, 2, 3, 4, 5]
};

const sugarSyrup = {
    white: ['1/8oz','1/4oz','1/2oz','5/8oz','3/4oz']
    demarara: ['1/8oz','1/4oz','1/2oz','5/8oz','3/4oz']
}


const myPerfectOldFashioned = { 
  whiskey: { name: "Michter's 10 Year Rye", proof: 92.8, flavorProfile: ['Rich Spice', 'Oak'], yearsAged: 10, ounces: 2 }, 
  sugar: ['demerara', 1]
};

```

## Bitters

Have you ever seen a raondom white bottle with the label sticking out as if the bottle is too big for it? Yellow top and black lettering reading **ANGOSTURA BITTERS**.
Well thats bitters for you. Some random guy in the world decided it was a good idea to take a bunch of herbs, spices, fruits and make a little tinchure: a concentration of whatever flavors came into his head. 
Normally they were used for medicinal purposes, however later in the 1800s a bartender decided it wasa  good idea to use it add another layer of flvor to a drink. FYI; it was a good idea!
today there are many types of bitters and anyone can pretty much make them using anything they want to flavor, just add everclear to whatever flavors you want to be infused, let it concentrate for god knows how long, taste, let time pass, tasete again, let more time pass and eventually
you will end up with a mixture filled with a unit flavor. Add some distiled water to open it up (decrease the alcohol amount so that the flavors can come out) and BAM your own bitters.

A list of poppular used bitters round the world...

**Angostura Bitters:** Created in 1824 by a german physician Johann Gottlieb Benjamin Siegert, in a random town west bumble f venezula to treat stomach aliment. He later commerciallied it in 1830 and overtime it grained popularity world wide. 
*Flavor Profile:* Bittersweet, warm spices, cinnamon, clove, hint of citrus and orange peels

**Peychaud Bitters:** When you think of New Orleans, it’s an alcoholic's dream. 24-hour open container? Sign them up! But a lot of cocktail culture, its origins, as well as its rich history, takes place in New Orleans. This type of bitters is probably the second most used worldwide after Angostura, but it was created by a Creole apothecary named Antoine Amedie Peychaud. Like the German physician, he too used it to aid digestion, but us revolutionaries found a better use for it. Peychaud's bitters was then born.
*Flavor Profile:* Anise is the domiment flavor, however you also get notes of cherry, refreshing herbs, hints of citrus and a sudtle hint of winter spices. 

**Orange Bitters:**  History is a little unknown but like the name, orange its main flavor profile is orange, citrus, dry, peels

### Overview

In the end, these add significant more flavors to drinks. Notable cocktails liek a ***sazerac*** (rye old fashioned with peychayd bitters), a ***Queens Park Swizzle*** (Mojito with all the bitters) have remain staples to this day but we can all thank bitters for that. Now you have ***Celery bitter***, ***Grapefruit bitter***, ***Chocolate bitter***, ***Coffee bitter*** and many many more. 

```js
// use this object to add your bitters!

const bitters = {
    Angostura: [1 dashes,2 dashes,3 dashes,4 dashes,5 dashes,6 dashes,7 dashes,8 dashes],
    Peychaud: [1 dashes,2 dashes,3 dashes,4 dashes,5 dashes,6 dashes,7 dashes,8 dashes],
    Orange: [1 dashes,2 dashes,3 dashes,4 dashes,5 dashes,6 dashes,7 dashes,8 dashes],
}

const myPerfectOldFashioned = { 
  whiskey: { name: "Michter's 10 Year Rye", proof: 92.8, flavorProfile: ['Rich Spice', 'Oak'], yearsAged: 10, ounces: 2 }, 
  sugar: ['demerara', 1],
  Angostura: [6 Dashes],
};

```

## ICE
Is water and ice important? Just watch this video, and you'll know everything you need to know. Learn from the [Ice king](https://www.youtube.com/watch?v=ET8mqVGDQ1s&t=3s) himself.

## ITS ALIVE
Now let's bring it all in. Garnishes are usually an orange peel or a lemon peel. As you can see, an old fashioned is very relative. There are all these things that you can use to make it, from the whiskey to the sugar and even the bitters you decide on. Some places will use Angostura and orange bitters; some will use simple syrup or demerara sugar, or even rye or bourbon. It will all vary; your standard recipe is...

> **2 oz** Bourbon <br> 
> **3 Dashes** Angostura <br> 
> **1** White Sugar Cube <br> 
> Splash of Club Soda <br>

**Instructions:** Add bitters, sugar, and splash of club soda to a glass and muddle until dissolved. Add ice followed by the whiskey of choice and garnish with orange and lemon peel.

**MY PERSONALLY PREFERRED RECIPE IS:** <br>
>  **2 oz** Mitchers 10 Year <br> 
>  **4 Dashes** Angostura <br> 
>  **2 Dashes** Orange <br> 
>  **1** Brown Sugar Cube <br> 
>  Splash of Club Soda <br>

This is my personal preference, but in the end, yours might be different. Play around, expand your horizons; hopefully, this inspires you to venture into the unknown. Let it all start with a glass and end with a great story. Enjoy!


