
# musicard-quartz 🎵

The kawaii 💕 npm package for generating sugoi 🤩 music cards for your apps and sites! 

```
npm install musicard-quartz
```

This package is a fun fork of musicard with some radical new features 🌈 for maximum sugoi-ness!


## Usage

Generate a quartz card like normal:

```js
(async () => {
    const { musicCard } = require("musicard-quartz");
    const fs = require("fs");

    const card = new musicCard()
        .setName("Aduh")
        .setAuthor("Maliq & D'Essentials")
        .setColor("auto")
        .setTheme("quartz+")
        .setBrightness(50)
        .setThumbnail("https://cdn.discordapp.com/attachments/1198220352963219456/1202316791351615548/index.jpg?ex=65cd03c5&is=65ba8ec5&hm=d5229d21023379c157e7e9bfa7d0258e6bcf7d7727a2381d133d51d3498bd3bf&")
        .setProgress(10)
        .setStartTime("0:00")
        .setEndTime("3:00")

    const cardBuffer = await card.build();

    fs.writeFileSync(`musicard.png`, cardBuffer);
    console.log("Done!");
})();
```

Here's a preview:

This is the **quartz+** output of musicCard. 
![quartz+](https://i.imgur.com/Ej0fR2G.png)

This is the **onepiece+** output of musicCard. 
![onepiece+](https://i.imgur.com/W1aKxlA.png)

This is the **vector+** output of musicCard. 
![onepiece+](https://i.imgur.com/Ej0fR2G.png)


Original musicard package by [RAMON](https://github.com/hymoonz/musicard-quartz)
