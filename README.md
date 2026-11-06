README.md

I haven't had time to upload the code, so let me guide you by drafting what I
am working on.

fluid is made up of mutliple pieces:

- datafirst / homeless
  btrfs like data storage with JSON like format with shared changelog
  on multiple devices

  ROADMAP:
    [x] prototype done
    [working] fuse testing
    [planned] typing /derived contents

  MySQL like have binary logs which can be used to move a database to another
  system fast. Wordpress/Vite/ .. AI now blurs the line: data (database)/code
  _> recompile -> web AI can do all. So we need new tools to reflect that.

  Users have mutliple devices and don't want to get stuck recalling where
  something is. It should just float to the destination and be usable .. :/
  
  By having conflict resoultion and JSON like data on file system level
  getting colaborative editing and perfect retriggering of rebuilds 
  will fix many existing issues on different levels

  Any industry apps like Blender, storytold etc will be added on top of this
  allowing open source community to add their own more

- fluid-compiler
  TS is gradual in typing. Yet the IT universe is scattered into many
  ecosystems and pieces. AI doesn't fix because somebody still must tell what
  to do and review and test. So multiple languages still slow down.

  Gradual compiler which can compile down to
  - dynamic targets JS/PHP/Python/Ruby
  - compiled targets Go/C
  - WASM
  - eventually ownership (Rust like)
    -> this kinda will come with all pros /cons of Rust
    -> this just means sliding into Rust is easier but probably
    will only eventually still compile to other targets

  Think abou this way {"name": "Ben", "data": NativeRustType(type, ptr)}
  How dynamic and compiled lanugages will interact.

  Examples which will get simplified due to using same ecosystem:
    - micropython (dense .py + .py -> on microcontroller)
    - vite / JS packaging (esbuild + webpack)
    - opencv (C++ + python)
    - Rust + scripting
    - mixing Wordpress/Vite
      -> installing a plugin will optimize and compile the code
      and reach Go/Rust level memory and CPU footprints !

  If there was one last surving programming lanugage being fittest
  serving embedded, scripting, shell, web ... this shall come closest

- dependency system

  There is brew, apt, nixos, guix, .. what you want is
  recipe -> use native what's available -> add the rest -> build & run or
  create package for all platforms including MS Windows.

  Think about it to be github README with contains a machine readable format about
  how to install on your system and graphic card

  => This enables even seing projects like Wordpress + PHP as "file" whic can be moved
  cause the target system will install the required dependencies automatically.

  ROADMAP: (working)
  [x] py integrated with different GPU types
  [x] rust integrated
  [x] HGo integrated
  [x] some c integrated

  targeting (working)
  [x] nixpkgs
  [x] compile yourself in directory
  [x] bucky2

  More ecos systems and targets coming

They all will also create workspaces treating code as data so that you can
creatively build whatever AI based pipeline you have in mind.

Later I also want to create own hardware which will basicaly be a CPU/GPU/NPU
with switchable display: no=clock, small=mobile, big=desktop, eink=outdoor,
2=vr

Additionally I want to start a Youtube channel to show off my progress and
expose myself to the world to engage the masses.
