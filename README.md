# card-game

A small Java Swing desktop app created as a high-school project. The user can choose among three classic card games: Blackjack, Sette e Mezzo, and Solitario. The GUI handles game selection, card draws, scoring, and restarts using local deck images.

## 📑 Index

- [Key Features](#-key-features)
- [Prerequisites](#-prerequisites)
- [Installation](#-installation)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [Configuration (Environment Variables)](#-configuration-environment-variables)
- [Contributing](#-contributing)
- [License](#-license)

## ✨ Key Features

- Simple Java Swing GUI for a school project
- Three games: Blackjack, Sette e Mezzo, and Solitario
- Supports French and Triestine decks
- Card images loaded from local folders
- Restart and score display per game

## 🛠 Prerequisites

- Java JDK [version]
- (Optional) Eclipse IDE to import the existing project files

## 🚀 Installation

```bash
# 1. Clone the repository
git clone [https://github.com/your-user/card-game.git](https://github.com/your-user/card-game.git)

# 2. Enter the directory
cd card-game

# 3. Compile the sources
javac -d bin $(find src -name "*.java")
```

If you use Eclipse, import the project as an existing project (files .project and .classpath are present).

## 💻 Usage

```bash
# Run the main class
java -cp bin it.volta.ts.marinollilorenzo.setteemezzo.boundary.Main
```

Example from code:

```java
new Console().esegui();
```

After launch, choose a game and follow the GUI buttons (Pesca, Sto, Restart).

## 📁 Project Structure

```plaintext
card-game/
├── src/                          # Java sources
│   └── it/volta/ts/...            # Packages
├── bin/                          # Compiled classes (generated)
├── CARTEFRANCESI/                # French deck images
├── CARTETRIESTINE/               # Triestine deck images
├── .project                      # Eclipse project file
└── .classpath                    # Eclipse classpath
```

## ⚙️ Configuration (Environment Variables)

No environment variables are required.

Note: the code expects deck folders named `carteFrancesi` and `carteTriestine`. On case-sensitive file systems, either rename the folders to match those names or update the paths in `Config.setDeckPath()`.

## 🤝 Contributing

- Fork the project
- Create a feature branch (`git checkout -b feature/NewFeature`)
- Commit your changes (`git commit -m "Add NewFeature"`)
- Push the branch (`git push origin feature/NewFeature`)
- Open a Pull Request

## 📄 License

Distributed under the [License Name, e.g. MIT]. See LICENSE for details.
