# Fastfetch #

## Preview : ##
<div allign=center>
<img width="1504" height="609" alt="Image" src="https://github.com/user-attachments/assets/f9f59718-9d86-45dc-ab36-0c639120139e" />
</div>

## <a name=logo></a>Logo ##
The logo is animated using kitty icat, therefore **you need kitty terminal** to use gif as logo.

Here is how you create your own animated logo:
```
# Locate your logo.gif for an example in ~/Downloads/logo.gif then use this command to convert it to bin so it can be used inside config.jsonc
kitten icat -n --align=left --transfer-mode=stream ~/Downloads/logo.gif > ~/.config/fastfetch/logo/image.bin
```
You can save it as any name you like but the extension must be .bin so the raw mode for logo recognize it

If you change it for an example to mylogo.bin then **don't forget to change the source inside `config.jsonc`**

For an example:
```
...
{
  "logo": {
    "type": "raw",
    "source": "~/.config/fastfetch/logo/mylogo.bin", // change this to the output you choose when running the kitten icat command
    "padding": {
      "top": 2
    }
  },
...
```

## How to use it ##
Just run this to have the config inside your fastfetch config:
```
git clone https://github.com/Adsani/fetch.git ~/.config/fastfetch
```
The default logo is a Still In Love headpat from Uma Musume, if you want to change it, [it's up here](#logo)

## Prerequisite ##
- Kitty terminal (If you don't want the gif as logo, you can skip it, but you may need to change the logo setting inside `config.jsonc`)
- Any font with nerd font symbol

That's it, hope you like my modified fastfetch config

## Credit ##
Feel free to use or share any part of this. If you do, a link back to this repo is appreciated. It’s just dotfiles, so nothing too serious
