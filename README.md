## Hello, welcome to my profile!

### About me:
```nix
{ config, pkgs, lib, ... }:

let
  present = builtins.trace "you are here" true;
in
{
  user = {
    name = "Synghuan";
    username = "foundingrain";
    location = "University at Albany";
    role = "MS CS Student";
  };

  about = {
    description = ''
      Hey, it's ${config.user.name}.
      I do a lot of different things like modding games, trying to make art, and doing fun little programming projects!
      I enjoy messing with 3D models in unity / blender, homelabbing, and creating new things to share with the world!
      This profile attempts to declare my current state.
    '';
  };

  time = {
    past = "immutable";
    current = present;
    future = "lazily evaluated";
  };

  languages = [
    "Nix"
    "C"
    "C#"
    "Java"
  ];

  tools = [
    "Linux.NixOS"
    "Microsoft.Windows"
    "Hackintosh.OSX"
    "React"
    "Avalonia"
    "SDL3"
    "Blender"
    "Unity"
    "Ford.Mustang"
  ];

  hobbies = {
    technical = [
      "programming"
      "open source"
      "linux"
      "amateur radio"
      "homelabbing"
    ];

    creative = [
      "drawing"
      "3D texturing"
      "game modding"
    ];

    recreational = [
      "driving"
      "video editing"
      "fpv drone piloting"
    ];
  };

  programs = {
    git.enable = true;
    neovim.enable = true;
    niri.enable = true;
    fish.enable = true;
  };

  services = {
    caffeine.enable = true;
    sleep.enable = false;
  };

  warnings =
    lib.optional config.services.sleep.enable
      "WARNING: sleep.enable overrides caffeine.enable. Enable with caution..";

  system.stateVersion = "2026.03";
}
```
<!--
**foundingrain/foundingrain** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
