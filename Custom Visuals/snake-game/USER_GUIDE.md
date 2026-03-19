# Snake Game - User Guide

## Overview

The Snake Game is a custom Power BI visual that brings the classic Snake arcade game directly into your Power BI reports. Navigate the snake to eat food, grow longer, and rack up the highest score — all without leaving your dashboard. It's a fun easter egg to embed in reports for team engagement or simply to take a quick break between data analysis sessions.

## Installation

1. Download the `snakegame67E5AB03A75446EDB26ED4A06034576C.1.0.0.0.pbiviz` file from this repository
2. In Power BI Desktop, click the ellipsis (...) in the Visualizations pane
3. Select "Import a visual from a file"
4. Navigate to and select the downloaded `.pbiviz` file
5. Click "OK" to confirm the import

## Getting Started

### Adding the Visual to Your Report

1. Click the Snake Game icon in the Visualizations pane
2. Resize and position the visual on your report canvas
3. Click on the visual to give it focus
4. Use the arrow keys or WASD keys to start playing

> **Note:** This visual does not require any data fields — simply add it to your report and start playing.

## How to Play

### Controls

| Key | Action |
|---|---|
| **Arrow Up** / **W** | Move up |
| **Arrow Down** / **S** | Move down |
| **Arrow Left** / **A** | Move left |
| **Arrow Right** / **D** | Move right |

### Rules

- The snake moves continuously in the current direction
- Eat the food (colored dot) to grow longer and increase your score
- Avoid hitting the walls or the snake's own body
- The game ends when the snake collides with a wall or itself
- Press any direction key to restart after a game over

### Scoring

- Each food item collected adds to your score
- The snake grows longer with each food item, increasing the challenge
- Try to beat your high score each round

## Use Cases

### Team Engagement
- Add to a hidden report page as an easter egg for your team to discover
- Use as a fun break during long dashboard review sessions
- Include on a "Fun" or "About" page in team-facing reports

### Presentations & Demos
- Use as an icebreaker during Power BI presentations or training sessions
- Demonstrate that Power BI custom visuals can render any interactive content, not just charts
- Showcase the flexibility of the Power BI custom visuals framework

### Gamification
- Embed alongside KPI dashboards to reward teams who hit their targets
- Add to a celebratory report page triggered by milestone achievements
- Use as a lighthearted addition to internal team dashboards

## Best Practices

### Report Design
- **Dedicated space** — give the visual enough room on the canvas for comfortable gameplay (minimum 400x400 pixels recommended)
- **Separate page** — consider placing the game on its own report page or a hidden page to keep it separate from business data
- **Focus mode** — users can expand the visual to full screen using the Focus Mode option for a better experience

### Performance
- The visual is lightweight and does not consume data model resources
- No dataset queries are made — all game logic runs client-side in the browser
- Adding the visual has no impact on report refresh performance

## Troubleshooting

**Issue**: Snake is not responding to keyboard input
- Click directly on the visual first to give it focus
- Ensure no other visual or UI element has captured keyboard focus
- Try clicking inside the game area and then pressing a direction key

**Issue**: Visual appears blank or does not load
- Verify the `.pbiviz` file was imported successfully (check the Visualizations pane for the icon)
- Try removing and re-adding the visual to the report canvas
- Ensure you are using a supported version of Power BI Desktop

**Issue**: Game area is too small
- Resize the visual on the report canvas to give it more room
- Use Focus Mode (click the expand icon in the visual header) for a full-screen experience

**Issue**: Game runs too fast or too slow
- Game speed may vary based on browser/system performance
- Try closing other resource-intensive applications or browser tabs

## Technical Requirements

- Power BI Desktop (latest version recommended)
- No dataset or data fields required
- Keyboard input required for gameplay (not available on touch-only devices without a keyboard)
- Supported in Power BI Desktop and Power BI Service (web browser)

## Support and Feedback

For issues, questions, or feature requests:
- Visit: http://powerbiwall.com/PBI-visuals
- Repository: https://github.com/PBI-Nathan/powerbi-resources

## Version Information

**Current Version**: 1.0.0.0

**Change Log**:
- Initial release with classic Snake gameplay
- Arrow key and WASD control support
- Score tracking
- Collision detection (walls and self)
