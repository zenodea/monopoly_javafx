# Monopoly Game - JavaFX

A fully functional Monopoly board game implementation built with JavaFX, featuring both human and AI players.

## Features

- **Complete Monopoly Gameplay**: All standard Monopoly rules implemented
- **JavaFX GUI**: Modern, interactive graphical user interface
- **AI Players**: Intelligent computer opponents with strategic decision-making
- **Property Management**: Buy, sell, mortgage, and develop properties
- **Card System**: Chance and Community Chest cards with various effects
- **Multiple Player Support**: Support for multiple human and AI players
- **Dice Rolling**: Realistic dice mechanics with visual feedback

## Requirements

- Java 17 or higher
- JavaFX 17.0.2
- Maven 3.6+

## Installation & Setup

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd monopoly_javafx
   ```

2. Install dependencies:
   ```bash
   mvn clean install
   ```

3. Run the game:
   ```bash
   mvn javafx:run
   ```

## Project Structure

```
src/
├── GUI/                    # User interface components
│   ├── GUI.java           # Main game interface
│   ├── Launcher.java      # Application entry point
│   └── PlayerInformation.java # Player info display
├── backend/               # Game logic
│   ├── Board.java         # Game board management
│   ├── Player/            # Player implementations
│   │   ├── Player.java    # Base player class
│   │   ├── HumanPlayer.java # Human player implementation
│   │   └── AI/            # AI player system
│   ├── Tiles/             # Board tile implementations
│   └── Exception/         # Custom game exceptions
└── resources/             # Game assets (images, JSON configs)
```

## Game Components

### Tiles
- **Properties**: Buyable properties with rent and development options
- **Utilities**: Electric Company and Water Works
- **Railroads**: Four railroad stations
- **Special Tiles**: Go, Jail, Free Parking, Go to Jail, Tax tiles

### Cards
- **Chance Cards**: Random events and actions
- **Community Chest**: Community-based events

### Players
- **Human Players**: Interactive gameplay with GUI controls
- **AI Players**: Computer-controlled with strategic decision making

## Configuration

Game configuration is stored in JSON files:
- `Tiles.Json`: Board tile definitions
- `LuckCard.Json`: Chance card definitions  
- `OpportunityCard.Json`: Community Chest card definitions

## Testing

Run the test suite:
```bash
mvn test
```