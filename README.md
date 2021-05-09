![Logo](https://camo.githubusercontent.com/b0ab1106f079aac465f467de9f6339656c5a5977dd31da1d6551836c89c639b8/68747470733a2f2f67697463646e2e6c696e6b2f7265706f2f686f70736f66742f7374696d756c75735f7265666c65782f6d61737465722f6173736574732f7374696d756c75732d7265666c65782d6c6f676f2d776974682d636f70792e737667)

    
# Stimulus Reflex Sandbox

Based on [SR Mini](https://github.com/hopsoft/sr_mini)



[![Remix on Glitch](https://cdn.gomix.com/f3620a78-0ad3-4f81-a271-c8a4faa20f86%2Fremix-button.svg)](https://glitch.com/edit/#!/remix/stimulus-reflex-sandbox)
## Tech Stack

- Ruby 3.0.1
- Rails 6.1.3.2
- *StimulusReflex* 3.4.1
- *CableReady* 4.5
- Redis 6.2.2
- **NO** database

  
## Usage/Examples


  
## FAQ/Gotchas

#### Help! My app is stuck in an install loop

Occasionally, building the assets via snowpack will fail, so you'll have to open the Glitch terminal (bottom left under *Tools*):

![Toolbar Screenshot](https://cdn.glitch.com/5d1b65f4-c468-4b36-bfe5-74a6315b9984%2FCleanShot%202021-05-09%20at%2014.11.00%402x.png?v=1620562298119)

and run

```bash
$ rm -rf node_modules
```

Your container will restart, installing fresh node modules, and the app should start correctly.

#### DB/Peristence/ActiveRecord

**There is no database**, due to the minimal and ephemeral nature of Glitch apps. However, [nulldb](https://github.com/nulldb/nulldb) is included so any persistence calls to ActiveRecord won't blow up the demo.

Feel free to emulate persistence using the `session` or Redis. If you feel adventurous, you can connect your sandbox to any external managed DB, though.

  
## Authors

- [@julianrubisch](https://www.github.com/julianrubisch)
- [@hopsoft](https://www.github.com/hopsoft)
- [@leastbad](https://www.github.com/leastbad)

  
## License

[MIT](https://choosealicense.com/licenses/mit/)

  