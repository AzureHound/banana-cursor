# NixOS Installation Instructions

To install this package on NixOS is rather easy.

First, you'll need to make a custom derivation. You use find the banana-cursor.nix inside of this repo.

Then inside of your home manager, you can define your cursor as follows:

```
home.pointerCursor = {
  package = pkgs.banana-cursor;
  name = "Banana-Catppuccin-Macchiato";
  size = 96;
  gtk.enable = true;
  x11.enable = true;
};
```

Additionally, you'll also want to set this up for any other window manager you might be using
