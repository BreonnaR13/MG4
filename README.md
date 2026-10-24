# MG4
## Devlog

To make the fish food objects go up and down, FloatAnimation utilizes the Start() method, Update() method, _up variable, and _timer variable. First when the Start() method is called _timer is set to _switchSpeed which is a float that has a value of 3.0. In the Update() method that runs each frame, with the use of Time.deltaTime, the _timer variable decreases by the amount of time that goes by. When the value of _timer is less than or equal to 0, it resets the _timer value to _switchSpeed. Also there is a variable called _up. _up starts off with the default value of false. Then in Update(), if _up is false the fish food objects are translated in the y-axis using the negative product of the _moveSpeed variable and Time.deltaTime to ensure that the fish food goes downwards. When up() is equal to true it would be a y-axis translation without the negative so that it goes up. The up() switches from true to false or vice versa when the _timer variable is less than or equal to 0.

## Open-Source Assets
- [Quirky animal 3D models](https://assetstore.unity.com/packages/3d/characters/animals/quirky-series-free-animals-pack-178235)
- [City 3D models](https://assetstore.unity.com/packages/3d/environments/simplepoly-city-low-poly-assets-58899)
- [Bite sound effect](https://freesound.org/people/Jofae/sounds/353067/)