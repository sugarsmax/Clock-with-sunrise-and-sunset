# 24-Hour Sunrise Sunset Clock Project

## Project Overview

A web-based 24-hour clock that displays the current time with an hour hand, plus two additional hands showing sunrise and sunset times. The clock is designed with noon positioned at the top.

## Repository

- **GitHub Repo**: https://github.com/sugarsmax/Clock-with-sunrise-and-sunset.git
- **Live Demo**: https://sugarsmax.github.io/Clock-with-sunrise-and-sunset/

## Requirements (Original Request)

- 24-hour clock face
- Only an hour hand for current time
- One hand for sunrise indication
- One hand for sunset indication
- Noon positioned at the top of the clock

## Features Implemented

- **24-hour format** with proper hour markers
- **Three hands**:
  - White hour hand (current time) - moves continuously
  - Orange sunrise hand (fixed position based on sunrise time)
  - Orange/red sunset hand (fixed position based on sunset time)
- **Hour markers** with major markers at 12, 6, 18, and 24 (midnight)
- **Real-time updates** every second
- **Digital time display** showing current time and sunrise/sunset times
- **Legend** to identify each hand
- **Responsive design** that works on various screen sizes

## Technical Details

### File Structure

```
/
├── index.html          # Main clock application (single file)
└── README.md          # This documentation
```

### Technologies Used

- HTML5
- CSS3 (with gradients and animations)
- Vanilla JavaScript
- No external dependencies

### Current Configuration

- **Sunrise**: 6:30 AM
- **Sunset**: 6:45 PM
- **Update interval**: 1 second

## Development Process

### Initial Discussion

- Started with question about Cursor for iPad
- Discussed project storage and development workflow for iPad users
- Established GitHub repo for version control

### Implementation

- Created single HTML file with embedded CSS and JavaScript
- Positioned noon at top (12 o’clock position)
- Implemented 24-hour markers with 15-degree intervals
- Added three hands with different colors and purposes
- Included real-time updates and digital display

### Deployment

- Used GitHub Pages for live hosting
- Accessed via: Settings > Pages > Deploy from branch > main

## Customization Options

### Changing Sunrise/Sunset Times

You can modify the times in two ways:

1. **Edit the variables** (around line 115):

```javascript
let sunriseTime = { hour: 6, minute: 30 }; // 6:30 AM
let sunsetTime = { hour: 18, minute: 45 }; // 6:45 PM
```

1. **Use the setSunTimes function**:

```javascript
setSunTimes({ hour: 7, minute: 15 }, { hour: 19, minute: 30 });
```

### Color Customization

- **Hour hand**: White (#fff)
- **Sunrise hand**: Orange (#ff6b35)
- **Sunset hand**: Orange-red (#ff8c42)
- **Background**: Blue gradient
- **Major markers**: Gold (#ffd700)

## Future Enhancement Ideas

- [ ] Location-based sunrise/sunset calculation
- [ ] Seasonal sunrise/sunset variation
- [ ] Different time zones
- [ ] Mobile app version
- [ ] Custom color themes
- [ ] Sound notifications at sunrise/sunset
- [ ] Weather integration

## Development Workflow for iPad Users

### Tools Used

- GitHub web interface for repo management
- GitHub Pages for hosting
- Web browser for testing

### Recommended Workflow

1. Make changes in GitHub web editor
1. Commit changes
1. View updates on GitHub Pages URL
1. Document changes in this README

## Conversation Summary

This project emerged from a discussion about development tools for iPad users. We explored:

- Cursor availability for iPad (not available)
- Project storage and collaboration methods
- GitHub workflow for iPad development
- HTML/CSS/JavaScript implementation
- GitHub Pages deployment
- Documentation best practices

## Resources and References

- [GitHub Pages Documentation](https://pages.github.com/)
- [HTML Canvas Clock Tutorials](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)
- [CSS Transform Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/transform)

## License

Open source - feel free to use and modify

-----

*Created: [Current Date]*  
*Last Updated: [Current Date]*  
*Platform: iPad-friendly development*
