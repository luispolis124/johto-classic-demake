# Pokémon Johto Classic

A modernized Pokémon Crystal demake patch based on the `pret/pokecrystal` disassembly, crafted via Termux and distributed via xdelta.

## About

**Pokémon Johto Classic** is a custom ROM hack project that brings a fresh retro perspective to Gen 2, built cleanly from source using modern decompilation tools. Instead of distributing copyrighted ROM files, this project uses `.xdelta` patches to keep development open-source and legal.

## Requirements

To play this hack, you will need:
* A clean base ROM: **Pokémon - Crystal Version (USA, Europe) (Rev 1).gbc**
* A patch applicator tool (such as [Delta Patcher](https://www.romhacking.net/utilities/704/) or [Lunar IPS](https://www.romhacking.net/utilities/240/))
* A Game Boy Color emulator (e.g., Gambatte, BGB, RetroArch, or Pizza Boy)

## How to Apply the Patch

1. Download the latest `johto_classic_vX.X.xdelta` file from the [Releases](../../releases) page.
2. Download or locate a clean copy of the required base ROM (**Pokémon - Crystal Version (USA, Europe) (Rev 1.gbc**).
3. Open a patcher tool like Delta Patcher.
4. Select your clean base ROM as the **Original file**.
5. Select the downloaded `.xdelta` file as the **XDelta patch**.
6. Click **Patch** to generate your playable `Pokémon Johto Classic.gbc` file.

## Building from Source (Termux / Linux)

If you are a developer looking to compile the source code or contribute using Termux:

1. Install dependencies:
   ```bash
   pkg update && pkg install git build-essential rgbds xdelta3

 * Clone the repository:
   git clone [https://github.com/luispolis124/pokemon-johto-classic.git](https://github.com/luispolis124/pokemon-johto-classic.git)
cd pokemon-johto-classic

 * Place your clean baserom.gbc (Rev 1) in the root directory.
 * Compile the ROM:
   make

 * Generate a new xdelta patch:
   xdelta3 -e -s baserom.gbc pokecrystal.gbc johto_classic_v1.0.xdelta

Credits & Special Thanks
 * pret team for the incredible pokecrystal disassembly project.
 * Game Freak / Nintendo for creating the original Pokémon Crystal.

