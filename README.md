Godot - https://godotengine.org/
with its native extension thing - https://docs.godotengine.org/en/stable/tutorials/scripting/gdextension/what_is_gdextension.html
which is available in version 4+
using the rust project - https://godot-rust.github.io/
that wraps / uses that GDExtension.

godot is installed via pacman on Archlinux.
rust things by installing rustup from pacman and setting up using stable.

Just trying to follow https://godot-rust.github.io/book/intro/index.html
to see how it feels.

proj/
  - godot    <--- godot project created here, open this one on the editor
  - rust     <--- rust code is here, cargo inside this folder

rust folder code becomes available as a c library, which godot project
then picks up using the file rust.gdextension that points to that artifact.

changing rust code and compiling, then opening godot inside the godot folder
and things become available.
