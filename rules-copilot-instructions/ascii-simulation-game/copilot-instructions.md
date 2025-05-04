# ASCII Simulation Game Copilot Instructions

## General Game Design & Programming
- You are an expert game designer and programmer; use best practices for all decisions.

## Core Game Mechanics
- The game is a 10x10 grid, each square has a 10x10 grid inside.
- Random map generation for resources, oceans, rivers, mountains, and neutral land.
- Player is an observer; provide logs for almost everything, turn-based.
- Nations are balanced, can trade, go to war, make peace, and expand via armies.
- Population lives in towns/cities, which grow and gather resources.
- Roads connect towns/cities and spread resources/gold.
- Armies are the main way to expand territory; spawn at towns/cities.
- No tech tree; ancient time period.
- Oceans, rivers, and mountains affect movement and resources.

## Army & Battle Mechanics
- Armies (level 1-10) require wood, food, metal; funded by nations.
- Battles use a RISK-like dice mechanic, affected by army level.
- Armies can build castles, conquer/defend squares, attack nations/neutral squares.
- Nations pay upkeep for armies and developed land.
- Nations start with equal gold and land.

## Data Tracking & Charts
- Provide a chart page tracking all game data.
- Maintain a battle list with stats.
- Allow viewing of map, square owners, resources, and game history/logs.

## Visual & Observational Rules
- Map is colored ASCII, showing square owners.
- Screen effects mimic a CRT monitor.
- Simulation style is similar to Conway's Game of Life; nations "see" and react to each other/resources.

