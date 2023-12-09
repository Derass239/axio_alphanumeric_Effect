# <div align="center"># Axio alphabet and number in "fireworks" </div>

This is simple script to allow you to show some text using particle for FiveM

## Preview

![App Screenshot](https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExcWk4OWZoYnY5MWpqMGZtcjY5eThnMnBlNGU0dzh1YTJ5OGY4bmZnbiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/hMZwY64oebkhf8qZz1/giphy.gif)

## Exports

#### Show text
```
  ShowFireworkText
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `text` | `string` | **Required**. Your text |
| `pos` | `vector3` | **Required**. Coord |
| `rotation` | `number` | Rotation |
| `colors` | `table` | Colors { r = 0.0, g = 255.0, b = 0.0} |

#### Clear text

```
  StopFireworkText
```

## Exemple

```lua
  RegisterCommand("exemple", function(source, args)
	local pos = vector3(-1985.7747, -923.1492, 50.7287)
	exports["axio_alphanumeric_Effect"]:ShowFireworkText("HAPPY", pos, 30)
	Wait(1750)
	exports["axio_alphanumeric_Effect"]:StopFireworkText()
	exports["axio_alphanumeric_Effect"]:ShowFireworkText("NEW", pos, 30)
	Wait(1750)
	exports["axio_alphanumeric_Effect"]:StopFireworkText()
	exports["axio_alphanumeric_Effect"]:ShowFireworkText("YEAR", pos, 30)
	Wait(1750)
	exports["axio_alphanumeric_Effect"]:StopFireworkText()
	exports["axio_alphanumeric_Effect"]:ShowFireworkText("2024", pos, 30)
	Wait(1750)
	exports["axio_alphanumeric_Effect"]:StopFireworkText()
end)

```

## Limitation

#### Available character
```
  ABCDEFGHIJKLMNOPQRTSUVWXYZ0123456789
```

#### Max character display at same time

In my tests, I was able to display up to 6 without problem, with more certain particles missing

# **Discord**

<a href="https://discord.gg/HPD35pasA5" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/discord.svg" alt="HPD35pasA5" height="120" width="180" /></a>

# LICENSE & DISCLAIMER

This repository was created by **Derass239** and is under the GNU General Public License v3.0 license.

❌ You are **not** allowed to sell this script or any of the content within it
