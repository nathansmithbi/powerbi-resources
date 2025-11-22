# Calendar Heatmap - User Guide

## Overview
The Calendar Heatmap is a custom Power BI visual that displays time-series data in a GitHub-style calendar grid format. Each day is represented by a colored cell, with color intensity indicating the value for that day. This visualization is ideal for showing activity patterns, trends, and distributions across days, weeks, and months.

![Calendar Heatmap](Images/Heatmap.png)

## Installation

1. Download the `.pbiviz` file from this repository
2. In Power BI Desktop, click the ellipsis (...) in the Visualizations pane
3. Select "Import a visual from a file"
4. Navigate to and select the downloaded `.pbiviz` file
5. Click "OK" to confirm the import

## Getting Started

### Adding the Visual to Your Report

1. Click the Calendar Heatmap icon in the Visualizations pane
2. Add a date column to the "Date" field well
3. Add a numeric measure to the "Value" field well
4. Resize and position the visual on your report canvas

### Basic Usage

The visual displays data in a calendar grid format where:

- **Each cell represents one day**
- **Color intensity indicates the value** for that day
- **Empty cells** represent days with no data
- **Month labels** appear at the top (when enabled)
- **Weekday labels** appear on the left (when enabled)
- **Year selector** allows navigation between different years
- **Play button** provides an animated reveal of the data

## Navigating the Calendar

### Year Selection

Click the year dropdown in the top-right corner to:
- View available years in your dataset
- Switch between different years
- The dropdown shows years in descending order (newest first)

### Animation

Click the play button to:
- Animate the appearance of data cells
- Watch the calendar fill in day by day
- Pause at any time by clicking the button again
- Speed can be adjusted in the Calendar Settings

### Tooltips

Hover over any cell to see:
- The date for that cell
- The value for that day
- "No data" indicator for empty cells
- Tooltips can be customized in Tooltip Settings

## Color Scale

The visual uses a color gradient to represent data values:

- **Empty Color**: Days with no data
- **Minimum Color**: Lowest values in the range
- **Maximum Color**: Highest values in the range
- **Gradient or Steps**: Choose between smooth gradient or discrete color levels

The legend at the bottom shows the color scale from "Less" to "More".

## Customization

### Calendar Settings

Access calendar settings in the Format pane (paint roller icon) under "Calendar Settings":

**Display Options:**
- **Show Year Selector**: Toggle the year dropdown (default: On)
- **Start Month**: Choose which month to start the calendar (1-12, default: 1 = January)
- **Number of Months**: How many months to display (1-24, default: 12)
- **Show Month Labels**: Display month names at the top (default: On)
- **Show Weekday Labels**: Display day abbreviations (Mon, Tue, etc.) (default: On)
- **Week Starts on Monday**: Start weeks on Monday instead of Sunday (default: Off)

**Cell Appearance:**
- **Cell Size**: Size of each calendar cell in pixels (default: 10)
- **Cell Padding**: Spacing between cells in pixels (default: 2)
- **Corner Radius**: Rounded corners for cells, 0-5 pixels (default: 2)

**Animation:**
- **Show Play Button**: Display the animation play button (default: On)
- **Animation Duration**: Time per cell reveal in milliseconds, 10-1000ms (default: 50)

### Color Settings

Customize colors in the Format pane under "Colors":

**Cell Colors:**
- **Empty Cell Color**: Color for days with no data (default: #ebedf0)
- **Minimum Value Color**: Color for lowest values (default: #c6e48b)
- **Maximum Value Color**: Color for highest values (default: #196127)
- **Use Gradient Scale**: Smooth color transition vs discrete steps (default: Off)
- **Color Steps**: Number of color levels when not using gradient, 2-10 (default: 5)

**Borders and Background:**
- **Cell Border Color**: Border color for cells (default: #ffffff)
- **Border Width**: Width of cell borders in pixels (default: 1)
- **Background Color**: Overall visual background (default: #ffffff)

### Label Settings

Customize text appearance in the Format pane under "Label Settings":

**Typography:**
- **Font Family**: Choose from Segoe UI, Arial, Calibri, Consolas, Courier New, Georgia, or Verdana (default: Segoe UI)
- **Month Label Size**: Font size for month names (default: 11)
- **Weekday Label Size**: Font size for day abbreviations (default: 11)

**Colors:**
- **Label Color**: Color for month and weekday labels (default: #586069)
- **Year Selector Text Color**: Color for year selector text (default: #586069)

### Title Settings

Add and customize a title in the Format pane under "Title":

- **Show Title**: Toggle title visibility (default: Off)
- **Title Text**: Custom text for the title (default: "Calendar Heatmap")
- **Font Size**: Title font size (default: 14)
- **Font Color**: Title text color (default: #586069)
- **Font Family**: Choose from available font families (default: Segoe UI)

### Tooltip Settings

Configure tooltips in the Format pane under "Tooltip Settings":

- **Show Tooltip**: Enable/disable tooltips (default: On)
- **Show Date in Tooltip**: Display the date (default: On)
- **Show Value in Tooltip**: Display the value (default: On)
- **Date Format**: Choose format (default: MMM dd, yyyy)
  - MM/DD/YYYY (e.g., 06/18/2025)
  - DD/MM/YYYY (e.g., 18/06/2025)
  - YYYY-MM-DD (e.g., 2025-06-18)
  - MMM DD, YYYY (e.g., Jun 18, 2025)
  - DD MMM YYYY (e.g., 18 Jun 2025)

## Use Cases

### Activity Tracking
Track daily activities, habits, or goals:
- Exercise frequency and intensity
- Study hours or reading time
- Task completion rates
- Meditation or health tracking

### Business Analytics
Analyze business metrics over time:
- Daily sales revenue or volume
- Customer support tickets
- Website visits or user engagement
- Transaction counts or values
- Order fulfillment rates

### Development & IT
Monitor technical metrics:
- Code commits (GitHub-style)
- Build success/failure rates
- Server uptime percentages
- API request volumes
- Bug reports or incidents

### Marketing & Social Media
Track engagement and reach:
- Social media posts and engagement
- Email campaign performance
- Content publication frequency
- Conversion rates by day

## Best Practices

### Report Design
- **Size Appropriately**: Ensure the visual is large enough to display all cells clearly
- **Use Consistent Colors**: Match your report theme for professional appearance
- **Consider Time Range**: Display 3, 6, or 12 months based on your analysis needs
- **Position Prominently**: Place where users can easily spot patterns

### Data Preparation
- **Daily Aggregation**: Ensure your data is aggregated to one value per day
- **Handle Missing Data**: Empty cells clearly show gaps in data collection
- **Date Column**: Use a proper date/datetime column in your dataset
- **Numeric Values**: Ensure values are numeric for proper color scaling

### Color Selection
- **High Contrast**: Choose min/max colors with sufficient contrast
- **Color Blindness**: Consider using color-blind friendly palettes
- **Background**: Use lighter backgrounds for better cell visibility
- **Gradient vs Steps**: Use gradient for continuous data, steps for categorical ranges

### Performance
- **Data Range**: Limit to necessary date ranges for better performance
- **Year Navigation**: Use year selector instead of showing multiple years at once
- **Cell Size**: Smaller cells perform better with large date ranges
- **Animation**: Adjust animation speed based on data density

## Troubleshooting

**Issue**: Visual is not displaying data
- Ensure a date column is in the Date field well
- Verify a numeric measure is in the Value field well
- Check that your date range includes data points
- Confirm the date column is formatted as Date or DateTime

**Issue**: All cells are the same color
- Check that your Value field contains varying numeric data
- Verify Minimum and Maximum colors are different
- Ensure you have more than one unique value in your dataset

**Issue**: Months are cut off or overlapping
- Increase the visual width
- Reduce the Cell Size setting
- Decrease the Number of Months displayed
- Reduce Cell Padding to create more space

**Issue**: Year selector is not showing all years
- Ensure your dataset contains data for those years
- Check that the date column includes the full date range
- Verify data is not filtered out by other slicers

**Issue**: Tooltip is not appearing
- Check that "Show Tooltip" is enabled in Tooltip Settings
- Ensure you're hovering over cells with data
- Verify your mouse is not moving too quickly

**Issue**: Animation is too fast or too slow
- Adjust "Animation Duration" in Calendar Settings
- Lower values = faster animation (10ms minimum)
- Higher values = slower animation (1000ms maximum)

## Technical Requirements

- Power BI Desktop (latest version recommended)
- A date or datetime column in your dataset
- A numeric measure for values
- Minimum visual size: 400px width x 300px height (recommended)
- Maximum recommended date range: 24 months

## Keyboard Navigation

- **Tab**: Navigate between interactive elements
- **Enter/Space**: Open year selector dropdown
- **Arrow Keys**: Navigate year options when dropdown is open
- **Escape**: Close year selector dropdown

## Support and Feedback

For issues, questions, or feature requests:
- Visit: http://powerbiwall.com/PBI-visuals
- Repository: https://github.com/PBI-Nathan/powerbi-visuals-calendar-heatmap

## Version Information

**Current Version**: 1.0.0.0

**Change Log**:
- Initial release with core calendar heatmap functionality
- Year selector with dropdown navigation
- Animation play button
- Customizable colors, fonts, and layouts
- Responsive tooltip system
- Support for gradient and stepped color scales
