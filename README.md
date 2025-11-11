# Pokedex

Command-line Pokemon exploration tool built in TypeScript/Node.js that allows users to explore the Pokemon world through an interactive REPL interface. The application integrates with the [PokeAPI](https://pokeapi.co) to fetch real-time Pokemon data.

This is the starter code used in Boot.dev's [Build a Pokedex in TypeScript](https://www.boot.dev/courses/build-pokedex-cli-typescript) course.

## Requirements

- Node.js 20+

## Installation

1. Clone the repository.

2. Install dependencies:
```bash
npm install
```

3. Build dependencies:
```bash
npm run build
```

## Usage

### Run the application
```bash
npm start
```

#### Example Session
##### Display help:
```bash
Pokedex > help
```
Output:
```bash
Welcome to the Pokedex!
Usage:
pokedex: Display the Pokedex
exit: Exit the Pokedex
help: Displays a help message
map: Displays a map of the Pokedex
mapb: Get the previous map of the Pokedex
explore: Explore area
catch: Catch a Pokemon
inspect: Inspect a Pokemon
```
##### View map:
```bash
Pokedex > map
```
Output:
```bash
canalave-city-area
eterna-city-area
pastoria-city-area
sunyshore-city-area
sinnoh-pokemon-league-area
oreburgh-mine-1f
oreburgh-mine-b1f
valley-windworks-area
eterna-forest-area
fuego-ironworks-area
mt-coronet-1f-route-207
mt-coronet-2f
mt-coronet-3f
mt-coronet-exterior-snowfall
mt-coronet-exterior-blizzard
mt-coronet-4f
mt-coronet-4f-small-room
mt-coronet-5f
mt-coronet-6f
mt-coronet-1f-from-exterior
```
##### Explore a location:
```bash
Pokedex > explore canalave-city-area
```
Output:
```bash
Exploring canalave-city-area...
Found Pokemon:
 - tentacool
 - tentacruel
 - staryu
 - magikarp
 - gyarados
 - wingull
 - pelipper
 - shellos
 - gastrodon
 - finneon
 - lumineon
```
##### Catch a Pokemon:
```bash
Pokedex > catch tentacool
```
Output:
```bash
Throwing a Pokeball at tentacool...
tentacool was caught!
```
##### View your Pokedex:
```bash
Pokedex > pokedex
```
Output:
```bash
Your Pokedex:
 - tentacool
```
##### Exit the application:
```bash
Pokedex > exit
```
Output:
```bash
Closing the Pokedex... Goodbye!
```

## Commands

| Command | Description |
|---------|-------------|
| `help` | Display a help message with all available commands |
| `exit` | Exit the Pokedex REPL |
| `map` | Display the next 20 location areas |
| `mapb` | Display the previous 20 location areas |
| `explore <location>` | List all Pokemon found in a specific location |
| `catch <pokemon>` | Attempt to catch a wild Pokemon |
| `inspect <pokemon>` | View detailed information about a caught Pokemon |
| `pokedex` | Display all Pokemon you've caught |
