# Pokémon Johto Classic

A modernized Pokémon Crystal demake patch based on the pret/pokecrystal disassembly, crafted via Termux and distributed via xdelta.
About
Pokémon Johto Classic is a custom ROM hack project that brings a fresh retro perspective to Gen 2, built cleanly from source using modern decompilation tools. Instead of distributing copyrighted ROM files, this project uses .xdelta patches to keep development open-source and legal.
Features & Progress
Here is the current implementation status of our custom features and systems:
 * ✅ Running Shoes System (Fast movement across maps)
 * ✅ Modernized pokecrystal Base (Clean assembly disassembling and compilation)
 * ✅ Termux Compatibility (Fully compiled and developed on mobile Android environment)
 * ❎ Full Pokémon Overworld Following System (Opted for streamlined companion mechanics due to hardware constraints)
 * ❎ Dynamic Weather Cycles (Planned for future post-jam updates)
Requirements
To play this hack, you will need:
 * A clean base ROM: Pokémon - Crystal Version (USA, Europe) (Rev 1).gbc
 * A patch applicator tool (such as Delta Patcher or Lunar IPS)
 * A Game Boy Color emulator (e.g., Gambatte, BGB, RetroArch, or Pizza Boy)
How to Apply the Patch
 * Download the latest johto_classic_vX.X.xdelta file from the Releases page.
 * Download or locate a clean copy of the required base ROM (Pokémon - Crystal Version (USA, Europe) (Rev 1).gbc).
 * Open a patcher tool like Delta Patcher.
 * Select your clean base ROM as the Original file.
 * Select the downloaded .xdelta file as the XDelta patch.
 * Click Patch to generate your playable Pokémon Johto Classic.gbc file.
Building from Source (Termux / Linux)
If you are a developer looking to compile the source code or contribute using Termux:
 * Install dependencies:
   pkg update && pkg install git build-essential rgbds xdelta3

 * Clone the repository:
   git clone https://github.com/luispolis124/johto-classic-demake.git
cd johto-classic-demake

 * Place your clean baserom.gbc (Rev 1) in the root directory.
 * Compile the ROM:
   make

 * Generate a new xdelta patch:
   xdelta3 -e -s baserom.gbc pokecrystal.gbc johto_classic_v1.0.xdelta

Credits & Special Thanks
 * pret team for the incredible pokecrystal disassembly project.
 * Tom Wang for the Running Shoes sprite implementation and foundational mechanics.
 * Game Freak / Nintendo for creating the original Pokémon Crystal.
