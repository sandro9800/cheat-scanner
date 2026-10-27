# CheatScanner

A lightweight Windows tool for scanning log and `.jar` files for suspicious Minecraft cheats and mods. CheatScanner started as a side project for my own server and is also a learning project.

> **Status: Beta.** Detection can miss cheats or produce false positives. Vape trace detection is especially unreliable, so treat results as clues to review rather than definitive proof.

## Features

- Scans log files and `.jar` files
- Checks for known cheat names, including Doomsday, Meteor, and Raven B++
- Looks for disguised or renamed mods
- Attempts to identify Vape traces (not reliable yet)

CheatScanner is a practical project in development, not a professional or guaranteed anti-cheat solution.

## Requirements

- Windows
- .NET 10 SDK to build and run the project from source

The project uses WPF and targets `net10.0-windows`.

## Build and run

Clone the repository and build the solution:

```bash
git clone https://github.com/sandro9800/cheat-scanner.git
cd cheat-scanner
dotnet build AntiCheatScanner.sln --configuration Release
```

You can also run the application from source with:

```bash
dotnet run --project AntiCheatScanner.csproj
```

Use the application to scan the log or `.jar` files you want to inspect. Review findings in context; a detection alone does not prove that a player is cheating.

## Feedback and contributions

Found a bug, a false positive, or a missed detection? Open a GitHub issue with details that are safe to share. Do not upload private logs or other sensitive data without removing it first.

Contributions and suggestions are welcome. Please keep changes focused and explain how you tested them.

## Contact

Discord: **Iobidze**

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for the license text. Third-party dependencies and other included material remain subject to their own licenses.